# aix-tests

See the `ansible.cfg` in this repo for parameters you might need to tweak

See `invengtory.aix` for host/group vars you might need to set

Run the following commands against the AIX hosts

Determine what facts are available by default
`ansible -m setup -i inventory.aix all`

Determine if privelege escalation is possible
`ansible -m shell -b -a "id" all`

Please run through the modules in this page to see if they work
https://www.djouxtech.net/posts/ansible-on-aix/

Determine if scan jobs with custom facts modules, fact scripts  can be run against AIX hosts in Tower.  Try and run the job templates associate with RHEL5/7 fact gathering.
