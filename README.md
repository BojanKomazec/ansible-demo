# ansible-demo
Repository contains various demo Ansible playbooks.

To run playbooks use ansible-playbook or ansible-navigator:
```
$ ansible-playbook ./run_locally/hello_world.yaml
$ ansible-navigator run ./run_locally/hello_world.yaml --mode stdout
```

To run test playbooks e.g. `test_install_docker_engine.yaml`:
```
$ ansible-playbook ./playbooks/tests/test_install_docker_engine.yaml --ask-become-pass --verbose
```

To install minikube locally:
```
$ ansible-playbook ./playbooks/run_locally/install_minikube.yaml --ask-become-pass --verbose
```

# Notes

If you need to use pipe (`|`) operator in order to pipe the output of one command into another then use `ansible.builtin.shell` instead of `ansible.builtin.command`.
