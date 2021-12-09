# epg-lifecycle

WARNING:

These scripts are meant for educational/proof of concept purposes only. Any use of these scripts and tools is at your own risk. There is no guarantee that they have been through thorough testing in a comparable environment and I am not responsible for any damage or data loss incurred as a result of their use.

Update inventory-file and variables.yaml for your credentials, APIC IP and policy settings

The playbook will create Interface Policy Groups, associate them with a Leaf Selector, create tenant policies and a static path binding.

To create/modify:
ansible-playbook -i inventory-file demoApp.yaml -e @variables.yaml

To remove:
ansible-playbook -i inventory-file demoApp.yaml -e @variables.yaml -e state_cli=absent
