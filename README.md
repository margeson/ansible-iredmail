# ansible-iredmail
Deploy iRedMail using Ansible - LetsEncrypt, Monit, Slack Notifications and FTP Backup

This playbook has been tested with Ubuntu 16.04

In its current state, iRedMail is deployed using Postges as the backend. 

The monit configuration requires Slack for alert notifications. And, the monit configs could use some tweaking. 

Feel free to contribute!

1. Save `config.yml.sample` as `config.yml`
2. Modify `config.yml`
3. Add your public key(s) to `authorized_keys`
4. Update `hosts` with the IP address of the instance you are deploying to
5. `ansible-playbook deploy.yml -i hosts`
