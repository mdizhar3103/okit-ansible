# Configuring OKIT with ansible
This repo contains the ansible playbook to configure oracle [OKIT](https://github.com/oracle/oci-designer-toolkit) locally.

***Note: The playbook is supported to run on RedHat or CentOS based distro with distribution version equal to or higher than 8, the default docker version is also specified update the version in variables if required of your choice.***

Pre-requisite to successfully run the playbook:
- Configure OCI config setup __.oci__, if oci cli is not installed the playbook install the oci-cli and later on the playbook will fail because of .oci not setup, then configure the oci config and re-run the playbook. 
- ssh keys are generated already in __.ssh__ folder

**Running the playbook**
```bash
# check oci config setup is success
oci os ns get

# Running the playbook
ansible-playbook okit.yml
```
