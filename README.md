# Kubernetes-Single-Node-Cluster-using-MicroK8s

The smallest, fastest, fully-conformant Kubernetes that tracks upstream releases and makes clustering trivial. MicroK8s is great for offline development, prototyping, and testing. Use it on a VM as a small, cheap, reliable k8s for CI/CD. The best Kubernetes for appliances. Develop IoT apps for k8s and deploy them to MicroK8s on your Linux boxes.

#What you’ll need

1- An Ubuntu 18.04 LTS or 16.04 LTS environment to run the commands 
   (or another operating system which supports snapd - see the snapd documentation)

2- At least 20G of disk space and 4G of memory are recommended

3- An internet connection

#Reference 
https://microk8s.io/docs/

#Note 
*microk8s.docker command not found*

If you used sudo snap install microk8s --classic command to install. Currently it will download v1.14.0.
You can check your version using #snap info microk8s

Version 1.14.0 introduced changes in microk8s.daemon-docker and change it to microk8s.daemon-containerd. Due to this change microk8s cannot execute docker commands. Microk8s contains daemon-docker between versions 1.11 and 1.13.

If you are used to use docker install microk8s v1.13 by sudo snap install microk8s --classic --channel=1.13/stable

