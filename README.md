## Ansible Role: Filebeat 
Role for installing and configuring Filebeat on the Elastic Stack
## Requirements
Ansible version: 2.9
Centos 7/ Debian
## Dependencies
None
## Example Playbook
```
- hosts:  "{{ var }}"
  vars:
    filebeat_output_elasticsearch_enabled: true
    filebeat_output_elasticsearch_hosts:
      - "10.1.10.250:9200"
    filebeat_username: elastic
    filebeat_password: "1234567890"
  roles:
    - ansible-role-filebeat
```

