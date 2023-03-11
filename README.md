# K8-s


# Flannel network

nano fannel.yml
copy paste the below content and save file
kubectl delete -f fannel.yml
kubectl apply -f fannel.yml
kubectl get pods -A

Create this file  /run/flannel/subnet.env manually as empty file and retry
cd /run
sudo mkdir  flannel
sudo vi /run/flannel/subnet.env 


FLANNEL_NETWORK=192.168.0.0/16
FLANNEL_SUBNET=192.168.0.1/24
FLANNEL_MTU=8951
FLANNEL_IPMASQ=true

