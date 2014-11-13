## Test playbook on vagrant

Configure .ssh/config, add host vagrant

    Host vagrant
        HostName 127.0.0.1
        User vagrant
        Port 2222
        UserKnownHostsFile /dev/null
        StrictHostKeyChecking no
        PasswordAuthentication no
        IdentityFile /Users/cecep/.vagrant.d/insecure_private_key
        IdentitiesOnly yes
        LogLevel FATAL

Edit/create new file, named ansible.cfg

    vi path-to/ansible-role-ntp/ansible.cfg

Content of ansible.cfg

    # file ansible.cfg
    [defaults]
    roles_path = ../

Run playbook

    ansible-playbook -i test/vagrant test/vagrant.yml


## Travis CI

READ: [Testing Ansible Roles with Travis CI on GitHub](https://servercheck.in/blog/testing-ansible-roles-travis-ci-github)
