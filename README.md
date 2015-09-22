# demo-ansible
An example Ansible playbook to be used w/ Jenkins
----
This repository is intended to act as a *simple* example for tracking
an Ansible playbook under version control and using that playbook with
the Jenkins-Ansible plugin.

Content description:

* ping_playbook.yml  -- the main playbook
* scloud_inventory   -- an inventory file for sCloud

Both of these files are referenced from the Jenkins job, which also
tracks this repository for changes.  

The Jenkins server is configured with credentials for the `build`
user.  The playbooks hardcode the username.  More advanced playbooks
would parametertize role account names and pass those parameters in
from the CLI or Jenkins.
