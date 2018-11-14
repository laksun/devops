Reference: http://blog.hortonew.com/ansible-splunk-forwarder-deployment

Made changes: 
1. On task "name: Push RPM package to server", owner and group changed to root
2. On task  "name: Start splunk",  "--answer-yes --auto-ports --no-prompt" is added to the shell command


Ansible commands:

ansible-playbook -i inventory SplunkUniversalForwarderInstallLinux.yml

You can use "--skip-tags server-config"  in the command if the splunk server is not reachable

Note:
   You need to download the correct splunkforwarder and copy it to the /tmp/ directory.
