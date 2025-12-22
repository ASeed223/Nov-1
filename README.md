. Preparation
login to lxadm101

cd OCP-Pipeline

git pull

decrypt

2. Configuration (Repeat for each environment)
cd deployments/ets-dev1

vi tpf-ui-config-maps.properties

Add this line: JBOSS_UI_AUTH_METHOD=KEYCLOAK-SAML

vi kustomization.yaml (Add the new properties file to the list)

3. Deploy & Verify
mkdir TpfTemp

oc kustomize . -o TpfTemp

npre ets-dev1

ls -1 *tpf-ui* | while read file; do oc apply -f $file; done;

Note: Repeat the above steps for UIT1, TST1A, and TST1B.
