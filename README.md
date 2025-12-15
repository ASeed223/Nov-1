# =========================================================
# 1. Clear old aliases (Required to make the function work)
# =========================================================
unalias status 2>/dev/null
unalias start 2>/dev/null
unalias stop 2>/dev/null

# =========================================================
# 2. Define custom Nexus status function (Mimics Systemd)
# =========================================================
status() {
    # Find Nexus Process ID (PID)
    local PID=$(ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep | awk '{print $2}' | head -n 1)

    echo "● nexus.service - Sonatype Nexus (User Space)"
    
    if [ -n "$PID" ]; then
        # Process exists, calculate start time and memory usage
        local START_TIME=$(ps -p $PID -o lstart=)
        local MEM_KB=$(ps -p $PID -o rss= | tr -d ' ')
        local MEM_MB=$(($MEM_KB / 1024))
        
        # Print green status "active (running)"
        echo -e "   Loaded: loaded (/etc/systemd/system/nexus.service; enabled; vendor preset: disabled)"
        echo -e "   Active: \033[32mactive (running)\033[0m since $START_TIME"
        echo -e " Main PID: $PID (java)"
        echo -e "   Memory: ${MEM_MB}M"
        echo -e "           └─$PID /opt/nexus/nexus/bin/../jvm/bin/java ..."
    else
        # Process missing, print red status "inactive (dead)"
        echo -e "   Loaded: loaded (/etc/systemd/system/nexus.service; enabled)"
        echo -e "   Active: \033[31minactive (dead)\033[0m"
    fi
}

# =========================================================
# 3. Define Start and Stop shortcuts
# =========================================================
alias start='/opt/nexus/nexus/bin/nexus start'
alias stop='/opt/nexus/nexus/bin/nexus stop'
