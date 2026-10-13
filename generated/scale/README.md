
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:e6545b198162ca7c364bb4eb72907dc1bc00b214f10d1a96bf98030b9dfdc54d
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:d515ec4b6cb4a25ce5d3d26dfa52ccfa94673d2dcd81c4b00bcb69620a0271f2 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:551b427af85ea4d046ff616d668dbe6edf91aaa9bcb770bc2d54986c64da493c |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:551b427af85ea4d046ff616d668dbe6edf91aaa9bcb770bc2d54986c64da493c |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:3fc33c7b6a05f149b0d6c96aa80f4104ab9321d93bb709b1eb546593cfc35f47 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:1bd8a8a28e3e6debce2970df4025baa912034f72a01b63ea87dc23ab7637f427 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:5f7b922121869c95553f48a72b09082530d85bd7cb4f2b709989b7ee32e70035  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:b4367111125f86a2a9a484532c731defab3c6fe10756454e26bb37e813ffd42f |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:9704b69af8761adad3d30ac335f1836f918eefae8c2948c0b94339593faebdab |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:996d0920e4ff9df1fc19dacb904492f3c1ec0ec1cc338f0ad7123be7731c5f5e |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:5f7b922121869c95553f48a72b09082530d85bd7cb4f2b709989b7ee32e70035 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:9616073fc8087915af5a371f831ed0aa880b08dbfa3f04b192952766bd3806b8 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:9704b69af8761adad3d30ac335f1836f918eefae8c2948c0b94339593faebdab |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:42af0929bcd60a43499825c078a60ff0534e08af8fbeb283aa391be40feb9f3e  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:d1a26170efed45491074ca4545c81844eee2b9043fb885ac01fb4aed6f8b72d2 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:a4b0b1a37605b7b04a293e136edf7006ec1786a8eb3f4e5a945f81d667dcc371 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:19f2cf2f40e1987c7943945deca5f65cd4e4bf5cc0657fc78a5df131861578e8 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:b7fefd08651f00ac4df1a196ed4c621c2451fbb899297fe9fad9e36c667af0c0 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:ea1d25e23479000c7e8eeb92d827df66258df4e482ca054c5e7ce3fc0f5c41a5 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:e1b4d31a6329489133917b5848ad76a99b4716c65e47eaad92abbba34141be2e |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:b7f78519c98b6f48062b2082dbf711fda7168085f64b3605ae7a935abbdc7fb3 |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:0218c7b71baabec0a383a74b3c15e3f860be99dfd9301b8f3f1fccbd0587c481 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:e6545b198162ca7c364bb4eb72907dc1bc00b214f10d1a96bf98030b9dfdc54d
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:3fc33c7b6a05f149b0d6c96aa80f4104ab9321d93bb709b1eb546593cfc35f47
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:1bd8a8a28e3e6debce2970df4025baa912034f72a01b63ea87dc23ab7637f427
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:551b427af85ea4d046ff616d668dbe6edf91aaa9bcb770bc2d54986c64da493c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:0218c7b71baabec0a383a74b3c15e3f860be99dfd9301b8f3f1fccbd0587c481
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:b7f78519c98b6f48062b2082dbf711fda7168085f64b3605ae7a935abbdc7fb3
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:b4367111125f86a2a9a484532c731defab3c6fe10756454e26bb37e813ffd42f
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:5f7b922121869c95553f48a72b09082530d85bd7cb4f2b709989b7ee32e70035
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:9704b69af8761adad3d30ac335f1836f918eefae8c2948c0b94339593faebdab
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:9616073fc8087915af5a371f831ed0aa880b08dbfa3f04b192952766bd3806b8
cp.icr.io/cp/gpfs/postgres@sha256:996d0920e4ff9df1fc19dacb904492f3c1ec0ec1cc338f0ad7123be7731c5f5e
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:d515ec4b6cb4a25ce5d3d26dfa52ccfa94673d2dcd81c4b00bcb69620a0271f2
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:d1a26170efed45491074ca4545c81844eee2b9043fb885ac01fb4aed6f8b72d2
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:b7fefd08651f00ac4df1a196ed4c621c2451fbb899297fe9fad9e36c667af0c0
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:a4b0b1a37605b7b04a293e136edf7006ec1786a8eb3f4e5a945f81d667dcc371
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:ea1d25e23479000c7e8eeb92d827df66258df4e482ca054c5e7ce3fc0f5c41a5
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:42af0929bcd60a43499825c078a60ff0534e08af8fbeb283aa391be40feb9f3e
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:e1b4d31a6329489133917b5848ad76a99b4716c65e47eaad92abbba34141be2e
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:19f2cf2f40e1987c7943945deca5f65cd4e4bf5cc0657fc78a5df131861578e8
```
