# Ansible Content Collections EE Integration Tests

## Steps

- `git clone https://github.com/brahmanim/ee_testing`
- `cd ee_testing`
- `Update the relevant inventory file`
- `Login to RH VPN`
- `podman pull <the EE image that you create from your content collection repo>`
- `ansible-navigator run --eei <image name> site.yaml -i <relevant inventory> --mode=stdout`
