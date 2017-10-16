# demansi
Demo Ansible multi-site project

Use this project as a template for a production grade Ansible project.

Directory structure:
```
.
├── ansible.cfg
├── LICENSE
├── playbooks
│   ├── debugvars.yml
│   ├── group_vars
│   │   └── all
│   │       ├── 10_general
│   │       └── README.md
│   └── init.yml -> ../roles/init/playbook.yml
├── README.md
├── roles
│   └── init
│       ├── defaults
│       │   └── main.yml
│       ├── files
│       ├── handlers
│       ├── meta
│       │   └── main.yml
│       ├── playbook.yml
│       ├── README.md
│       ├── tasks
│       │   ├── add_role.yml
│       │   ├── add_site.yml
│       │   └── main.yml
│       ├── templates
│       │   ├── file.j2
│       │   ├── hosts.j2
│       │   ├── main_defaults.yml.j2
│       │   ├── main_meta.yml.j2
│       │   ├── main_meta.yml.orig
│       │   ├── main_tasks.yml.j2
│       │   ├── main_vars.yml.j2
│       │   ├── playbook.yml.j2
│       │   ├── README.md.j2
│       │   └── sitevars.j2
│       └── vars
│           └── main.yml
└── sites
    ├── dev
    │   ├── group_vars
    │   │   └── all
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
    │   ├── 01_setup
    │   ├── 05_security
    │   ├── 10_general
    │   ├── 20_network
    │   ├── 30_storage
    │   ├── 40_virt
    │   ├── 50_ha
    │   └── README.md
    ├── prod
    │   ├── group_vars
    │   │   └── all
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
        │       ├── 01_setup -> ../../../group_vars/01_setup
        │       ├── 05_security -> ../../../group_vars/05_security
        │       ├── 10_general -> ../../../group_vars/10_general
        │       ├── 20_network -> ../../../group_vars/20_network
        │       ├── 30_storage -> ../../../group_vars/30_storage
        │       ├── 40_virt -> ../../../group_vars/40_virt
        │       ├── 50_ha -> ../../../group_vars/50_ha
        │       └── 90_sitevars
        └── hosts

23 directories, 60 files
```
