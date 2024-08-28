# Flask Project

This project is set up to run a Flask application using Vagrant for environment management and Ansible for provisioning.

## Prerequisites
- Make sure you have [Vagrant](https://www.vagrantup.com/downloads) installed on your machine.
- Install [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) for provisioning the Vagrant environment.
- Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) to use as a provider for Vagrant.

## Getting Started

1. **Clone the Repository**
   ```bash
   git clone https://github.com/furkanekici/flask-project
   cd flask-project

2. **Set Up the Environment**
   ```bash
    vagrant destroy    # destroy any existing Vagrant environment
    vagrant up        # provision the Vagrant environment

 Vagrant will create a new virtual machine, provision it with the necessary dependencies, and deploy your Flask application using Ansible. 
 
3.  Once the provisioning is complete, you can access your Flask application by opening a web browser and navigating to http://localhost:5000.

