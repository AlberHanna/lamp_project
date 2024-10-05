# lamp_project
Automating LAMP Stack Deployment with Ansible

# LAMP Stack Deployment with Ansible

This project automates the deployment of a **LAMP (Linux, Apache, MySQL, PHP)** stack across multiple servers using Ansible. The playbook installs and configures Apache, MySQL, and PHP, deploys a sample PHP application, and connects it to a MySQL database.

## Project Overview

- **Web Server**: Apache and PHP will be installed.
- **Database Server**: MySQL will be installed and secured.
- **PHP Application**: A sample PHP script will be deployed on the web server to verify the connection to the MySQL database.

## Prerequisites

- **Ansible Control Node**: A machine with Ansible installed.
- **Target Nodes**: Multiple Linux servers to install Apache, MySQL, and PHP.
- **SSH Access**: Passwordless SSH access must be set up from the control node to the target nodes.

```lamp_project/
├── inventory
├── lamp_setup.yml
└── roles/
    ├── apache/
    │   └── tasks/
    │       └── main.yml
    ├── mysql/
    │   └── tasks/
    │       └── main.yml
    └── php/
        └── tasks/
            └── main.yml

