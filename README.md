# Elasticsearch Ansible Playbook

A simple Ansible Playbook to install and set up Filebeat, Elasticsearch and Kibana.

Additionally, a role to set up [oauth2\_proxy](https://github.com/bitly/oauth2_proxy) is provided, to provide authentication for Kibana.

Currently the playbook only runs on deb-based distribution.

## Usage

1. Copy `hosts.example` to `hosts` and edit it properly.
2. Optionally edit the vars in `site.yaml`. They can be overridden by `-e key=value`.
3. Run `ansible-playbook -i hosts site.yaml`.
