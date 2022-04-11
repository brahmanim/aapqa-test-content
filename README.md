# EE Test

## Steps

- `git clone https://github.com/NilashishC/ee_testing`
- `cd ee_testing`
- `Update the inventory file`
- `Login to RH VPN`
- `podman pull <image from Jira ticket>`
- `ansible-navigator run --eei <image> site.yaml -i inventory --mode=stdout`
