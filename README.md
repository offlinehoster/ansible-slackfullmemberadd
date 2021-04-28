# ansible-slackfullmemberadd

Slack is a platform for team communication

## What you can do with this role
------------------------------
You can simple integrate this role to your automation process, for example if a new employee is joining your team, you can just add this user by this Ansible role to your team.

Tunables
--------
Modifying the vars.yml with your prefered vars
* `name:` (string) - his/her name
* `surname:` (string) - his/her surname
* `email:` (string) - the users email for the invite
* `slackteamname:` (string) - your teamname at Slack
* `token:` (string) - your token for access this api (get/create it here https://api.slack.com/web)

## Dependencies
------------
nothing special - but you may use just the latest version of ansible if possible.

## Good to know
------------
This is not an official usage for the /api/users.admin.invite uri by Slack. It's working good since a while, so i decide to automate this process by using ansible.

Example Playbook
----------------
```
---
- name: ansible-slackfullmemberadd
  hosts: 127.0.0.1
  connection: local
  roles:
  - ansible-slackfullmemberadd
  tags:
  - ansible-slackfullmemberadd
```
## Ansible Galaxy Role
-------------------
[Ansible Galaxy Role ](https://galaxy.ansible.com/offlinehoster/slack_fullmemberadd)

## License
-------
[MIT](https://tldrlegal.com/license/mit-license)

## Contributors
------------
* Christian Sarazin
