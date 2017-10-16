# demansi
Demo Ansible multi-site project

Use this project as a template for a production grade Ansible project.

Directory structure:
.
├── ansible.cfg
├── LICENSE
├── playbooks
│   ├── debugvars.yml
│   ├── group_vars
│   │   └── all
│   │       ├── 00_README
│   │       └── 10_general
│   └── skeleton.yml -> ../roles/skeleton/playbook.yml
├── README.md
├── roles
│   └── skeleton
│       ├── defaults
│       │   └── main.yml
│       ├── files
│       ├── meta
│       │   └── main.yml
│       ├── playbook.yml
│       ├── tasks
│       │   └── main.yml
│       ├── templates
│       └── vars
│           └── main.yml
└── sites
    ├── dev
    │   ├── group_vars
    │   │   └── all
    │   │       ├── 00_README -> ../../../group_vars/00_README
    │   │       ├── 01_setup -> ../../../group_vars/01_setup
    │   │       ├── 05_security -> ../../../group_vars/05_security
    │   │       ├── 10_general -> ../../../group_vars/10_general
    │   │       ├── 20_network -> ../../../group_vars/20_network
    │   │       ├── 30_storage -> ../../../group_vars/30_storage
    │   │       ├── 40_virt -> ../../../group_vars/40_virt
    │   │       ├── 50_ha -> ../../../group_vars/50_ha
    │   │       └── 90_sitevars
    │   └── hosts
    ├── group_vars
    │   ├── 00_README
    │   ├── 01_setup
    │   ├── 05_security
    │   ├── 10_general
    │   ├── 20_network
    │   ├── 30_storage
    │   ├── 40_virt
    │   └── 50_ha
    ├── prod
    │   ├── group_vars
    │   │   └── all
    │   │       ├── 00_README -> ../../../group_vars/00_README
    │   │       ├── 01_setup -> ../../../group_vars/01_setup
    │   │       ├── 05_security -> ../../../group_vars/05_security
    │   │       ├── 10_general -> ../../../group_vars/10_general
    │   │       ├── 20_network -> ../../../group_vars/20_network
    │   │       ├── 30_storage -> ../../../group_vars/30_storage
    │   │       ├── 40_virt -> ../../../group_vars/40_virt
    │   │       ├── 50_ha -> ../../../group_vars/50_ha
    │   │       └── 90_sitevars
    │   └── hosts
    └── stage
        ├── group_vars
        │   └── all
        │       ├── 00_README -> ../../../group_vars/00_README
        │       ├── 01_setup -> ../../../group_vars/01_setup
        │       ├── 05_security -> ../../../group_vars/05_security
        │       ├── 10_general -> ../../../group_vars/10_general
        │       ├── 20_network -> ../../../group_vars/20_network
        │       ├── 30_storage -> ../../../group_vars/30_storage
        │       ├── 40_virt -> ../../../group_vars/40_virt
        │       ├── 50_ha -> ../../../group_vars/50_ha
        │       └── 90_sitevars
        └── hosts

