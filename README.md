# nginx-setup-role

# Prerequisites:
 Public key of control-host's user already added to managed's /root/.ssh/ directory
 Managed host OS is Ubuntu Server

 Vault pass is '12345'
 Web creds are:
                aaa/ ->  usera:a-pass
                
                bbb/ ->  userb:b-pass
# Run:

ansible-playbook nginx-setup.yml -i inventory --ask-vault-pass -u root
