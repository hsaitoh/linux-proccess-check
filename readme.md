# mem usage per proccess

```
$ ps -o pid,user,%mem,command ax | sort -b -k3 -r | more
   PID USER     %MEM COMMAND
 73768 21035     9.9 java -Xms2G -Xmx2G -XX:MaxMetaspaceSize=256m -XX:MetaspaceSize=256m -Xss1m -XX:ReservedCodeCacheSize=240m -XX:MaxDirectMemorySize=10m -XX:+UseG1GC -Djava.security.
egd=file:/dev/urandom -javaagent:/home/kzp00/agent.jar -Duser.timezone=Asia/Tokyo -jar /home/kzp00/waybillpdf.jar
  5524 root      1.4 /usr/local/bin/kubelet --enable-server --node-labels=node-role.kubernetes.io/agent=,kubernetes.io/role=agent,agentpool=nodepool1,storageprofile=managed,storagetier
=Standard_LRS,kubernetes.azure.com/cluster=MC_KZP-DEV-RSG_aks-e-dev-002_japaneast --v=2 --volume-plugin-dir=/etc/kubernetes/volumeplugins --address=0.0.0.0 --allow-privileged=true --an
onymous-auth=false --authorization-mode=Webhook --azure-container-registry-config=/etc/kubernetes/azure.json --cgroups-per-qos=true --client-ca-file=/etc/kubernetes/certs/ca.crt --clou
d-config=/etc/kubernetes/azure.json --cloud-provider=azure --cluster-dns=172.26.250.138 --cluster-domain=cluster.local --enforce-node-allocatable=pods --event-qps=0 --eviction-hard=mem
ory.available<750Mi,nodefs.available<10%,nodefs.inodesFree<5% --feature-gates=PodPriority=true,RotateKubeletServerCertificate=true --image-gc-high-threshold=85 --image-gc-low-threshold
=80 --image-pull-progress-deadline=30m --keep-terminated-pod-volumes=false --kube-reserved=cpu=89m,memory=2662Mi --kubeconfig=/var/lib/kubelet/kubeconfig --max-pods=30 --network-plugin
=cni --node-status-update-frequency=10s --non-masquerade-cidr=0.0.0.0/0 --pod-infra-container-image=aksrepos.azurecr.io/mirror/pause-amd64:3.1 --pod-manifest-path=/etc/kubernetes/manif
ests --pod-max-pids=-1 --protect-kernel-defaults=true --rotate-certificates=false --streaming-connection-idle-timeout=5m --tls-cert-file=/etc/kubernetes/certs/kubeletserver.crt --tls-c
ipher-suites=TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256,TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256,TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305,TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384,TLS_ECDHE_RSA_WI
TH_CHACHA20_POLY1305,TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384,TLS_RSA_WITH_AES_256_GCM_SHA384,TLS_RSA_WITH_AES_128_GCM_SHA256 --tls-private-key-file=/etc/kubernetes/certs/kubeletserver.
key
 73446 omsagent  1.3 /opt/microsoft/omsagent/ruby/bin/ruby /opt/microsoft/omsagent/bin/omsagent-229da045-ee8c-4a5f-81e9-6862564c6a2c -d /var/opt/microsoft/omsagent/229da045-ee8c-4a5f-8
1e9-6862564c6a2c/run/omsagent.pid --no-supervisor -o /var/opt/microsoft/omsagent/229da045-ee8c-4a5f-81e9-6862564c6a2c/log/omsagent.log -c /etc/opt/microsoft/omsagent/229da045-ee8c-4a5f
-81e9-6862564c6a2c/conf/omsagent.conf
 98684 root      1.0 agent run
 73883 21035    10.0 java -Xms2G -Xmx2G -XX:MaxMetaspaceSize=256m -XX:MetaspaceSize=256m -Xss1m -XX:ReservedCodeCacheSize=240m -XX:MaxDirectMemorySize=10m -XX:+UseG1GC -Djava.security.
egd=file:/dev/urandom -javaagent:/home/kzp00/agent.jar -Duser.timezone=Asia/Tokyo -jar /home/kzp00/waybillpdf.jar
```
