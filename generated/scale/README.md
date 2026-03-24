
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:3da81cfa43881a20d3eede93a41f710c905b91e735f899cc01cb8c9ce570380c
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:a9c18c3f77a8ae89647b238b6504422fabc5bdc0aa59f45a7e179e2472086ec4 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:402aedc2d6b487bd7bd6d8494fa4e08953c5921a25a7893de6c3c29a66f04179 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:402aedc2d6b487bd7bd6d8494fa4e08953c5921a25a7893de6c3c29a66f04179 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:543816a95e6f6e6e76640671228dcc713a42acbcc122bf7f23077e210e5c130a |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:03a63d1b500b6c50e6f5aab1aae97e0d3e5658e1ef9c8f909431e1091b44d132 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:c0d8156a277041e4c8eb7206c428a8c8a1728b5117dd3c91d8bfe6672349b42b  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:05a1bb16e7ca717b279935e9678a92eaec97b530878f307418e95171d9934d2b |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:856b7b4978382ecacfa8235cc80bc87e721f768ef6999c23f3e4a0db66c589f2 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:c0d8156a277041e4c8eb7206c428a8c8a1728b5117dd3c91d8bfe6672349b42b |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:61163d62fc93fef53bfbead12d0bbc32eebb612fa0dc3afe8e938bca318aac25 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:856b7b4978382ecacfa8235cc80bc87e721f768ef6999c23f3e4a0db66c589f2 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:dd589aa2abd408d2e9c8f6a0b001db27802f1c3175a95c54f7c2d4993f6ae8d4 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:d423ca26549177b434efddd1fb21932f31110c288cfd77a2390d3bdf8af8876d |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:d5f4690898d9468a22d92f6da530cd28966dffc4e8519de89236954a3815dd02 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:3da81cfa43881a20d3eede93a41f710c905b91e735f899cc01cb8c9ce570380c
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:543816a95e6f6e6e76640671228dcc713a42acbcc122bf7f23077e210e5c130a
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:03a63d1b500b6c50e6f5aab1aae97e0d3e5658e1ef9c8f909431e1091b44d132
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:402aedc2d6b487bd7bd6d8494fa4e08953c5921a25a7893de6c3c29a66f04179
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:d5f4690898d9468a22d92f6da530cd28966dffc4e8519de89236954a3815dd02
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:d423ca26549177b434efddd1fb21932f31110c288cfd77a2390d3bdf8af8876d
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:05a1bb16e7ca717b279935e9678a92eaec97b530878f307418e95171d9934d2b
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:c0d8156a277041e4c8eb7206c428a8c8a1728b5117dd3c91d8bfe6672349b42b
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:856b7b4978382ecacfa8235cc80bc87e721f768ef6999c23f3e4a0db66c589f2
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:61163d62fc93fef53bfbead12d0bbc32eebb612fa0dc3afe8e938bca318aac25
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:a9c18c3f77a8ae89647b238b6504422fabc5bdc0aa59f45a7e179e2472086ec4
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:dd589aa2abd408d2e9c8f6a0b001db27802f1c3175a95c54f7c2d4993f6ae8d4
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e
```
