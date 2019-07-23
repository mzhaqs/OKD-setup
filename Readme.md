1. brew install socat
2. Download OKD
3. Download and install Docker Edge for Mac
4. Docker Edge Desktop for MAC -> Daemon -> Insecure registries -> 172.30.0.0/16
5. Run docker run -it --rm --privileged --pid=host justincormack/nsenter1 /bin/sh -c 'mkdir -p /var/lib/kubelet/device-plugins'
6. oc cluster up
7. oc login -u system:admin
8. oc adm policy add-cluster-role-to-user cluster-admin admin
