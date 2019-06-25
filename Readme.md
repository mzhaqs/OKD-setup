1. Download OKD
2. Docker Desktop for MAC -> Daemon -> Insecure registries -> 172.30.0.0/16
3. Run docker run -it --rm --privileged --pid=host justincormack/nsenter1 /bin/sh -c 'mkdir -p /var/lib/kubelet/device-plugins'
4. oc cluster up
4. oc login -u system:admin
2. oc adm policy add-cluster-role-to-user cluster-admin admin
