# ansible-minecraft
Deploy and configure Minecraft server using Ansible

## Instructions
### Configure Deployment
Check the `./group_vars/all.yaml` file and apply desirable configurations. Keep in mind that plugins are supported in case of specifying URLs and names. 
 
 ### Configure Minecraft
 * To configure server properties modify the `./minecraft/templates/server.properties`.
 * To configure PaperMC specific server settings in `./minecraft/templates/paper.yml`.
 * To add the server icon replace `./minecraft/templates/server-icon.png` with 64x64 pixel image of png format.

### Deploy
```bash
ssh-add <ssh_key_path>
ansible-playbook default.yaml
```
