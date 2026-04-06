### Install ansible collection

```
ansible-galaxy collection install community.docker
```
### pipx

*pipx* installs each application in its own virtual environment (in this case ansible). You can find the location of the Ansible with:

```
pipx list
```

To access to the Virtual environment:

```
source ~/.local/share/pipx/venvs/ansible-core/bin/activate
```

and at the end run:

```
deactivate
```

#### Inject command to add a library to the Ansible environments:

```
pipx inject ansible-core requests # E.g. Requests library 
```