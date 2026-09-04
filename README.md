# SSH Keys

I Drop my **SSH public keys** matching my private SSH keys here.
Pull this repository to your local machine and add your public key to the
`authorized_keys` file on the server to enable passwordless SSH access.

## NOTICE
This repository is for my personal use and is **not** intended for public
sharing of SSH keys. Only public keys should be added to the `authorized_keys`
file. Please do not add your private or public keys to this repository, even if
somehow possible, as it is a security risk. If you need to share your private or
public keys, please do so through a secure channel.

## NOTICE #2
**Do not**, **ever** add these public keys to your `authorized_keys` file on your server.
These keys are for my personal use only and should not be used by anyone else.
If you need to add your own public key to your server's `authorized_keys` file,
please do so through Your own repository and do not use any of the keys in this
repository, as that would only grant me access to your server, if any, which is
not my intention and not in my list of things to do.

## Warning (to myself)!!!
**Do not** add your **private** key to this repository! Only public keys should
be added to the `authorized_keys` file. **This repository is public** and
**anyone can view** the contents of the `authorized_keys` file. This is not a
secure way to share private keys, but it is a convenient way to share public
keys for SSH access which is safe to do. No-one can do anything with these public
keys except allow me to log in to their server if they have my public key in
their `authorized_keys` file.

## Instructions
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/vihoma/ssh-keys.git
   ```
2. Navigate to the cloned repository:
   ```bash
   cd ssh-keys
   ```
3. Add your SSH public key to the `authorized_keys` file:
   ```bash
   cat ~/.ssh/id_rsa.pub >> authorized_keys
   ```
4. Commit and push your changes to the repository:
   ```bash
   git add authorized_keys
   git commit -m "Add my SSH public key"
   git push origin main
   ```
