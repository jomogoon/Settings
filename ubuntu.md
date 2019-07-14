

1. if sudo service ssh start not working with below error

    $ sudo service ssh start
    [sudo] password for user:
    * Starting OpenBSD Secure Shell server sshd
    Could not load host key: /etc/ssh/ssh_host_rsa_key
    Could not load host key: /etc/ssh/ssh_host_dsa_key
    Could not load host key: /etc/ssh/ssh_host_ecdsa_key
    Could not load host key: /etc/ssh/ssh_host_ed25519_key
                                                                                                                    [ OK ]
    $ ssh localhost
    Connection closed by 127.0.0.1 port 22


2. update and install
    $ sudo apt-get remove --purge openssh-server
    $ sudo apt-get update --fix-missing
    $ sudo apt-get install openssh-server

3. Warning: the ECDSA host key for 'myserver' differs from the key for the IP address '127.0.0.1'
    $ ssh-keygen -R '127.0.0.1'

    