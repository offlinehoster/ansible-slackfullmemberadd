# ansible-slackfullmemberadd

Slack is a platform for team communication

Tunables
--------
Modifying the vars.yml with your prefered vars
* `name:` (string) - his/her name
* `surname:` (string) - his/her surname
* `email:` (string) - the users email for the invite
* `slackteamname:` (string) - your teamname at Slack
* `token:` (string) - your token for access this api (get/create it here https://api.slack.com/web)

Dependencies
------------
nothing special

Good to know
------------
This is not an official usage for the /api/users.admin.invite uri by Slack. It's working good since a while, so i decide to automate this process by using ansible. 

Example Playbook
----------------
---
- name: ansible-slackfullmemberadd
  hosts: 127.0.0.1
  connection: local
  roles:
  - ansible-slackfullmemberadd
  tags:
  - ansible-slackfullmemberadd

License
-------
[MIT](https://tldrlegal.com/license/mit-license)

Contributors
------------
* Christian Sarazin
