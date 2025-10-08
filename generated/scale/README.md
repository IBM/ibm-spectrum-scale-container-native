
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:948846021d87acbda10af4510fb41c004c85ae778d3b9018c86b67a231511030 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:85b3dcb4f60d0e6b510f98a910d098006732b41a99f6b1e925d50e329c2616dd |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:cb4d36939ef903cf4b861b876efb571916f1437ff508c581258129d8665ae8c7 |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:95737415a00be5ffffb4a25d4ca66995d91cd9dfea92f27ae41f9535b11f2556 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:95737415a00be5ffffb4a25d4ca66995d91cd9dfea92f27ae41f9535b11f2556 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:2fda299f4f34fbd8909a18c3c86051ce796daf503a9dbf5f61a98e87525ff130 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:990be071a1e56ecadce595401e7c62b6d2224546a2a1318bd688c42dd9bceb34 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:8a88c9335ad72e51b87a9dff839e1d8a52e00b2206c0b76edc3c5e4165a9c9ab  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:de894862e6974e7972674a4738f7d788c16b1571d4b0faa3d60fa7fbcc457017 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:81f7781f6e96083dfbe291f9e3be6a7a45952314765b9604dd7324f3d104d4cc |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:8a88c9335ad72e51b87a9dff839e1d8a52e00b2206c0b76edc3c5e4165a9c9ab |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:8b73a06ade5c008c760b49bc120c01f78f5fa53ca01015625343a75cb1cd76dd |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:81f7781f6e96083dfbe291f9e3be6a7a45952314765b9604dd7324f3d104d4cc |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:47b29442f42f9eea44cee07d7ea78df67325953e66eecb69faeb6b4f9913fc6e |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:0cd51125e115685cc9a8e807f5e7409b6f44c7e104a0056a01d4d92542eea47c |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:948846021d87acbda10af4510fb41c004c85ae778d3b9018c86b67a231511030
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:2fda299f4f34fbd8909a18c3c86051ce796daf503a9dbf5f61a98e87525ff130
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:990be071a1e56ecadce595401e7c62b6d2224546a2a1318bd688c42dd9bceb34
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:95737415a00be5ffffb4a25d4ca66995d91cd9dfea92f27ae41f9535b11f2556
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:0cd51125e115685cc9a8e807f5e7409b6f44c7e104a0056a01d4d92542eea47c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:de894862e6974e7972674a4738f7d788c16b1571d4b0faa3d60fa7fbcc457017
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:8a88c9335ad72e51b87a9dff839e1d8a52e00b2206c0b76edc3c5e4165a9c9ab
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:81f7781f6e96083dfbe291f9e3be6a7a45952314765b9604dd7324f3d104d4cc
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:8b73a06ade5c008c760b49bc120c01f78f5fa53ca01015625343a75cb1cd76dd
cp.icr.io/cp/gpfs/postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:cb4d36939ef903cf4b861b876efb571916f1437ff508c581258129d8665ae8c7
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:85b3dcb4f60d0e6b510f98a910d098006732b41a99f6b1e925d50e329c2616dd
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:47b29442f42f9eea44cee07d7ea78df67325953e66eecb69faeb6b4f9913fc6e
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
