# ansible-demo
Repository contains various demo Ansible playbooks.

To run playbooks use ansible-playbook or ansible-navigator:
```
$ ansible-playbook ./run_locally/hello_world.yaml
$ ansible-navigator run ./run_locally/hello_world.yaml --mode stdout
```

To install minikube locally:
```
$ ansible-playbook run_locally/install_minikube.yaml --ask-become-pass --verbose
```
