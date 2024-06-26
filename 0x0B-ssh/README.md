# 0x0B. SSH

In this project we are provided with an Ubuntu server, living in a data center
far far away. The server is configured with a ssh public key we provided.
Using the server we learn about the Secure Shell Protocol.

## Mandatory

[0-use_a_private_key](./0-use_a_private_key)

- This bash script uses `ssh` to connect to a server using the private key
  `~/.ssh/school` with the user `ubuntu`.
- Requirements:
  - Only `ssh` single-character flags are allowed.
  - Using `-l` flag is forbidden.

[1-create_ssh_key_pair](./1-create_ssh_key_pair)

- Creates an RSA key pair, in the current directory.
- Requirements:
  - Name of the created private key must be `school`
  - Number of bits in the created key to be created `4096`
  - The created key must be protected by the passphrase `betty`

[2-ssh_config](./2-ssh_config)

- A SSH configuration file for a local SSH client.
- Requirements:
  - SSH client must be configured:
    - to use the private key `~/.ssh/school`
    - to refuse to authenticate using a password

## Advanced

[100-puppet_ssh_config.pp](./100-puppet_ssh_config.pp)

- A Puppet manifest to make changes to the SSH client configuration file.
- Requirements:
  - SSH client must be configured:
    - to use the private key `~/.ssh/school`
    - to refuse to authenticate using a password
