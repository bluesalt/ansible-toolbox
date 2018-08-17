An Ansible role to configure my own toolbox such as Git, Vim.

### Dependencies
None

### Tested Environment
* Ansible 2.3
* CentOS 6/7

### Installation

```
ansible-galaxy install bluesalt.toolbox
```

### Role Variables
All the available options are not mandatory at the moment. Default values could be  referenced from the [role's defaults directory](defaults/main.yml).


#### Vim

* Use customized vim repo

```
toolbox_vim_repo: https://github.com/bluesalt/DOTVim
```

* Specify list of users whom the vim is intended for.

```
toolbox_vim_users:
  - "{{ ansible_user }}"
  - root
```

#### Git

* Specify list of users who will use Git

```
toolbox_git_users:
  - "{{ ansible_user }}"
  - root
```

#### tmux
* Specify list of users who will use tmux

```
toolbox_tmux_users:
  - "{{ ansible_user }}"
  - root
```

### License
Apache 2.0

### Author Information

This role was created in 2017 by [Jeff Li](https://blog.jeffli.me)
