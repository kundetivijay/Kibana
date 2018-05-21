# Kibana
How to execute the playbook on Ubuntu server:
+++++++++++++++++++++++++++++++++++++++++++++++++++

1) Download the code from the github account.
2) Move the playbook file under /etc/ansible location. Since parameters are set accordingly in ansible.cfg file.
3) Copy the public key to the remote server where you want to install the ELK.
4) Modify the parameter "interface_name" in all file under group_vars directory.
               ansible_interfaces[1] ---> This value can be set from the setup module which will show the total number of interfaces and set accordingly.
5) Now run the playbook, ansible-playbook site.yaml
