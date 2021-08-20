# Mac terminal configuration guide

1. Install iTerm2, configure ZSH, Oh My Zsh and Powerlevel10k ([link](https://gist.github.com/kevin-smets/8568070))

## Git

### Configure SSH keys

Save the right key under ./ssh and set ssh-agent and execute these commands:

```bash
ssh-keygen #if new key is needed
eval $(ssh-agent)
ssh-add ~/.ssh/<private_key_file> 
```

Create a file ./ssh/config with the following content:

```bash
Host *
UseKeychain yes
```