#perl ${fullWinRepo}/configmgmt/pega/build-pega-ear.pl --localGitRepo="${fullWinRepo}" --bulkUploadBaseline=${BULK_UPLOAD_static} --pegaEarBaseline=${PEGA_EAR} ${DeployToNexus}

perl ${fullWinRepo}/java/arch/build/maven/maven-build.pl --localGitRepo=${fullWinRepo}/java  --skipUpdate --deploy --module=splash_screen --path=bpm/pega_ear/splash_screen --moduleBaseline=${PEGA_EAR}
perl ${fullWinRepo}/java/arch/build/maven/maven-build.pl --localGitRepo=${fullWinRepo}/java  --skipUpdate --deploy --module=pega-ear --path=bpm/pega_ear/ear_modules --bulkUploadBaseline=${BULK_UPLOAD_static} --moduleBaseline=${PEGA_EAR}
