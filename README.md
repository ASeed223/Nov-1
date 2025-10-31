Repository=EDRRELEASE
Version=${BuildRecordId}
Type=ear



echo "Repository=${Repository}"
echo "Version=${Version}"
echo "Type=${Type}"

if [ -z "${Version}" ]; then
  echo "ERROR: Version is empty. Check upstream trigger parameters."
  exit 1
fi

python /home/cmdeploy/sonatype/scan.py "${Repository}" "${Version}" ear
