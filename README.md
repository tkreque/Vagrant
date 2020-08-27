# Vangrant environment
This Vagrant environment was created as part of my labs with Vangrant + Terraform + Ansible.

###### Requirements
- Virtual Box 6.1.12 r139181 (Qt5.12.8)
- Vagrant 2.2.9
- Ansible 2.9.12
- Python 3.8.2
- pip 20.0.2 from /usr/lib/python3/dist-packages/pip (python 3.8)

## Folder tree
```
.
├── appservers
│   └── Vagrantfile
├── configs
│   ├── mykey
│   └── mykey.pub
├── README.md
└── terraform
    └── Vagrantfile

3 directories, 5 files
```

## Commands to run

- Is required to the VMs be able to share the folders.
`vagrant plugin install vagrant-vbguest`
- Is required to create mykey for ssh connections in the VMs.
`ssh-keygen -t rsa -f ./configs/mykey`
