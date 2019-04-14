## What's this?
This is a base role I use to manage some of my personal servers running Ubuntu 18.04.

## What does it do?
- Updates all installed packages, installs a few ones I need.
- Creates specified user with sudo and SSH privileges, applies specified SSH pubkey.
- Applies a few custom sysctl configurations.
- Applies a custom systemd-journald configuration.
- Applies a custom sshd configuration.
- Enables UFW with a default deny policy and allows SSH through.

## Variables
- `handle_kernel_install`: Install specified kernel (default: true)
- `kernel_kind`: What kernel and headers to install (default: virtual-hwe-18.04)
- `ssh_port`: SSH daemon port (default: 329)
- `ssh_username`: User to create on target (no default)
- `ssh_pubkey`: SSH public key (no default)
