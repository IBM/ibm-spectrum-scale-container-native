
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:2da577c189c248a228e1f662b9a83dcd12c0b575f4bf83b46915499ab3f6c204 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:d5a18f541e96ebc1578badb8cdb98cdb3bbcd258e014bd9c1834b0115a3bc79c |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:1abf3d8829740c6f49670a0cbe6ba29af88a96136940125e9fd6ab549b993b6c |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:f49c95ce53760e5a73564066cb7b84e22a27981191f4f6ce27698521e9525755 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:f49c95ce53760e5a73564066cb7b84e22a27981191f4f6ce27698521e9525755 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:4843026199b7823444d549cd72a27b227ebefa6e10793b5e0711a342552aa492 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:6dbd6c5afe12df97f2241e451d440cb964cce74195e9da4dbf9fe2d965799ca4 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:78c0c6381c38cb47bb71e3073ac736de25d5567271fd46cad146675ab9525e32  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:2dc497ccadd6627b05ec093b98237fc7ac8ab8a94ff92a4730b03debc886b368 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:c70d025433427b5cd24b1c6484b63acc1b6a505fe5818d78ba863683497a69a5 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:78c0c6381c38cb47bb71e3073ac736de25d5567271fd46cad146675ab9525e32 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:42f0edd52708aa99010481ce758d5a906203812b682eb0c2ddd5a54b792ac460 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:c70d025433427b5cd24b1c6484b63acc1b6a505fe5818d78ba863683497a69a5 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:231e0975d55feebb691809d35237887b749ecb861a3ae8836a6b9354133911eb |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:bd458eb67c2bcb108696224b5618200f472fd10738abe29b553e11ed279e2c5c |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:18058dc1e5ee3febb327a13d846fa80533de365788e3e03ed00e358ef45581ff |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:2da577c189c248a228e1f662b9a83dcd12c0b575f4bf83b46915499ab3f6c204
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:4843026199b7823444d549cd72a27b227ebefa6e10793b5e0711a342552aa492
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:6dbd6c5afe12df97f2241e451d440cb964cce74195e9da4dbf9fe2d965799ca4
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:f49c95ce53760e5a73564066cb7b84e22a27981191f4f6ce27698521e9525755
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:18058dc1e5ee3febb327a13d846fa80533de365788e3e03ed00e358ef45581ff
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:bd458eb67c2bcb108696224b5618200f472fd10738abe29b553e11ed279e2c5c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:2dc497ccadd6627b05ec093b98237fc7ac8ab8a94ff92a4730b03debc886b368
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:78c0c6381c38cb47bb71e3073ac736de25d5567271fd46cad146675ab9525e32
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:c70d025433427b5cd24b1c6484b63acc1b6a505fe5818d78ba863683497a69a5
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:42f0edd52708aa99010481ce758d5a906203812b682eb0c2ddd5a54b792ac460
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:1abf3d8829740c6f49670a0cbe6ba29af88a96136940125e9fd6ab549b993b6c
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:d5a18f541e96ebc1578badb8cdb98cdb3bbcd258e014bd9c1834b0115a3bc79c
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:231e0975d55feebb691809d35237887b749ecb861a3ae8836a6b9354133911eb
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
