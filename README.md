# ansible-minecraft
Deploy and configure Minecraft server using Ansible

## Instructions
### Configure Deployment
1. Specify `ansible_host=` parameter in `./host` file
1. Check the `./group_vars/all.yaml` file and apply desirable configurations.

 ### Configure Minecraft
1. To configure server properties modify the `./minecraft/templates/server.properties`.
1. To configure PaperMC specific server settings in `./minecraft/templates/paper.yml`.
1. To add the server icon replace `./minecraft/templates/server-icon.png` with 64x64 pixel image of png format.

### Deploy
```bash
ssh-add <ssh_key_path>
ansible-playbook default.yaml
```
