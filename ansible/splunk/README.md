Reference: http://blog.hortonew.com/ansible-splunk-forwarder-deployment

Made changes: 
1. On task "name: Push RPM package to server", owner and group changed to root
2. On task  "name: Start splunk",  "--answer-yes --auto-ports --no-prompt" is added to the shell command
