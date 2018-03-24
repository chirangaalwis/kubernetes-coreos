# kubernetes-coreos

## TL;DR

I hacked something together in order to create a Kubernetes cluster on CoreOS (or Container Linux) using Vagrant and Ansible.

If you keep reading, I’m going to talk to you about Kubernetes, etcd, CoreOS, flannel, Calico, Infrastructure as Code and Ansible testing strategies. It’s gonna be super fun.

If you want to try it:

    git clone https://github.com/sebiwi/kubernetes-coreos
    cd kubernetes-coreos
    make up

This will spin up 4 VMs: an etcd node, a Kubernetes Master node, and two Kubernetes Worker nodes. You can modify the size of the cluster by hacking on the Vagrantfile and the Ansible inventory.

You will need Ansible 2.2, Vagrant, Virtualbox and kubectl. You will also need molecule and docker-py, if you want to run the tests.

## You can find the articles related to this repository below:

- Kubernetes general architecure: https://sebiwi.github.io/blog/how-does-it-work-kube-1/
- Kubernetes networking: https://sebiwi.github.io/blog/how-does-it-work-kube-2/
- Infrastructure as code, tools of the trade: https://sebiwi.github.io/blog/how-does-it-work-kube-3/
- How to Ansible your CoreOS, and etc(d)!: https://sebiwi.github.io/blog/how-does-it-work-kube-4/
- Master and worker, at last!: https://sebiwi.github.io/blog/how-does-it-work-kube-5/
