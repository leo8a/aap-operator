# Ansible Role: AAP operator

[![CI](https://github.com/leo8a/aap-operator/actions/workflows/ci.yml/badge.svg)](https://github.com/leo8a/aap-operator/actions/workflows/ci.yml)

Installs the [AAP](https://access.redhat.com/documentation/en-us/red_hat_ansible_automation_platform/) operator on OpenShift clusters.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    aap_enable_cluster_scope: true
    aap_operator_namespace: "ansible-automation-platform"
    
    aap_hub_enabled: true
    aap_hub_file_storage_access_mode: ReadWriteMany
    
    aap_controller_enabled: true
    aap_controller_file_storage_access_mode: ReadWriteMany

## Dependencies

This role requires the `kubernetes.core` collection, and have been tested on an OpenShift cluster version 4.10+.

## Example Playbook

    - hosts: localhost
      gather_facts: false
      roles:
        - leo8a.aap_operator

## License

This role is released under the Apache 2.0 license. See the [LICENSE](LICENSE).

## Author Information

This role was created in 2022 by [Leo Ochoa](https://github.com/leo8a/).

## Contributors

This is the current list of folks in the `aap_operator` hall of ~~fame~~ contributors 🏆!

<a href="https://github.com/leo8a/aap-operator/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=leo8a/aap-operator"  alt=""/>
</a>

> Made with [contributors-img](https://contrib.rocks).
