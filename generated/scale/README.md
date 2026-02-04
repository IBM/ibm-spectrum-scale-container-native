
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:c0958ef1b8c48bdaec6b9b798334271e8c792f13ee272444f3ca9c3955d04f21 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:e7b3fe21f3a87b75c115f366af45b79a164808e812e9e05ab8ed5fe41f460fae |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:4114c2514b2ea26acbb34a8c7e9701a129236e6b192c67dc78779f690d8dd73f |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:da99a1ca87759bc97955e1bb6362e4eccc08ffaa1bcaf3ff2822184ba5a8ca59 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:da99a1ca87759bc97955e1bb6362e4eccc08ffaa1bcaf3ff2822184ba5a8ca59 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:c24a97bf8665c6b4f5f7586969103d570b6e9e8866a631a47d2645af32c194f4 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:922c3b0fbc2718a836297187b94c7de09392fb65b94e1f3eb2f6ab5a3f3b5e33 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:f567a866db1c78d081bd952525339c04a5a8435da99cb545d9ffc2a0dbaae04b  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:37dfbc4c85481e3392e2ee418947a11894833e230bb626b9e1719eaec5728062 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:443d2d62ac369258598657f52e2f00405897701e868f67d5eea9b88c41cab604 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:f567a866db1c78d081bd952525339c04a5a8435da99cb545d9ffc2a0dbaae04b |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:ff69995e2557a946b603611fee5ea2773cebc505b64ed96be00f258d299fd969 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:443d2d62ac369258598657f52e2f00405897701e868f67d5eea9b88c41cab604 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:1b7d11c7f07fe86d52dd990487e0dfa297366b69e2ff2fe6f2f62eae3779007b |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:aa2de56ca0ed4fb24bd697e58275642c0fe9847748986ebc66c0b7b5ca5675fe |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:bcad2bad5e0ec4629c1f3d8c6372674b94c1e82f7d8bdf950306668367eef765 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:c0958ef1b8c48bdaec6b9b798334271e8c792f13ee272444f3ca9c3955d04f21
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:c24a97bf8665c6b4f5f7586969103d570b6e9e8866a631a47d2645af32c194f4
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:922c3b0fbc2718a836297187b94c7de09392fb65b94e1f3eb2f6ab5a3f3b5e33
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:da99a1ca87759bc97955e1bb6362e4eccc08ffaa1bcaf3ff2822184ba5a8ca59
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:bcad2bad5e0ec4629c1f3d8c6372674b94c1e82f7d8bdf950306668367eef765
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:aa2de56ca0ed4fb24bd697e58275642c0fe9847748986ebc66c0b7b5ca5675fe
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:37dfbc4c85481e3392e2ee418947a11894833e230bb626b9e1719eaec5728062
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:f567a866db1c78d081bd952525339c04a5a8435da99cb545d9ffc2a0dbaae04b
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:443d2d62ac369258598657f52e2f00405897701e868f67d5eea9b88c41cab604
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:ff69995e2557a946b603611fee5ea2773cebc505b64ed96be00f258d299fd969
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:4114c2514b2ea26acbb34a8c7e9701a129236e6b192c67dc78779f690d8dd73f
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:e7b3fe21f3a87b75c115f366af45b79a164808e812e9e05ab8ed5fe41f460fae
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:1b7d11c7f07fe86d52dd990487e0dfa297366b69e2ff2fe6f2f62eae3779007b
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
