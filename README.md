myRepo="c:/gitrepos/build/${trimRelease}"
python -u ${gitMasterLoc}/configmgmt/tfs/setupGitRepo.py -r "$myRepo" -b "$trimRelease" -s "java" -t "false"

javaRepo="${myRepo}/java"
#EDR_MAVEN_SETTINGS=${javaRepo}/arch/build/maven/edr-settings.xml
ccperl ${javaRepo}/arch/build/maven/maven-build-all-ears.pl --localGitRepo=${javaRepo} --earBaseline=${JAVA_APPS} --buildType="both" ${DeployToNexus}

earBaseline=${JAVA_APPS} 
