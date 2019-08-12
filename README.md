# Ansible playbook to deploy a private docker registry

This playbook helps you deploy your own, private docker registry to host your own images, or to proxy web based images to an airgapped environment using Docker. (https://docs.docker.com/v17.09/registry/deploying/)

This playbook
- Installs pre-requisites for docker registry
- Creates a self signed cert for use in the registry server
- Deploys docker registry
- Pulls a list of docker images (a list of elasticsearch images atm)
- Tags and pushes these images into the docker registry

The playbook currently supports Debian and RedHat based linux distros 
