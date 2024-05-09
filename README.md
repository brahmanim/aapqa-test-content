# Ansible Content Collections downstream EE Integration Tests
This playbook is ment to be run with ansible-navigator or with AAP controller.
Variable target_name should be specified on inventory file, or as extra var.
The value should be a specific integration test target name,or pattern like "{{ 
collection_name }}_*".

## Steps

- `git clone https://github.com/ansible/aapqa-test-content.git`
- `cd aapqa-test-content`
- `Update the relevant inventory file`
- `Login to RH VPN`
- `podman pull <the EE image that you create from your content collection repo>`
- `ansible-navigator run --eei <image name> run_integration_tests.yaml -i <relevant inventory> --mode=stdout --pp never -vvv`
