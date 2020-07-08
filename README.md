# azure_ocp_prereq
Prepare a machine for installing OpenShift in azure government

Clone this project `git clone git@github.com:pekramp/azure_ocp_prereq.git`<br />
Change into the directory `cd azure_ocp_prereq`

**Vars (vars/main.yml)**<br />
ocp_release = the version of OCP you want to get ready to install <br />
prereq_packages = the packages that will be installed to prepare to run the installer

**REQUIRED**<br />
pullsecret.json - your pull secret for accessing the OpenShift installation files <br />
Go to https://cloud.redhat.com/openshift/install/azure/user-provisioned <br />
Download or copy pull secret and save it to vars/pullsecret.json

After everything is set and ready you are ready to run the playbook<br />
Run with `ansible-playbook  azure_pre-reqs.yml --ask-become-pass`
