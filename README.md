# NATS Streaming Ansible Role

NATS Streaming is a data streaming system powered by NATS, and written in the Go programming language.

## Installation

``` yaml
# requirments.yaml
- src: git@github.com:4lie/ansible-role-nats-streaming.git
  scm: git
  version: master
  name: nats-streaming
```

## Role Variables

``` yaml
nats_streaming_version: "0.18.0"
nats_streaming_config_template: "{{ playbook_dir }}/templates/nats-streaming-server.conf.j2"
nats_streaming_nats_server_url: "nats://127.0.0.1:4222"
```

## Example Playbook

``` yaml
- hosts: servers
  roles:
    - nats-streaming
```
