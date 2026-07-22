
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:907b1187b1e47e17a1392d38856731ced3da418645b023062e3cf292e6ee99eb |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:b98a23cabda8c19bb4e488f46487b9c17a319e12ca00d833d7de139ff373b8b9 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:dac18aafbd462e766ae4f1806284bf9c48a5496e65c52fe1f16877655a283b80 |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:00c6c0571d6b13176522ac357b72910af31f6cd698bca54ff90ad9e8ccffa1e3 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:00c6c0571d6b13176522ac357b72910af31f6cd698bca54ff90ad9e8ccffa1e3 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:2b97c8539b2fe8d7d6a276f839613fb6bfa57e902723d76ca998628693e4475e |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:464598f26343bb776752aa0bd6142e2d40c6b7384875b0e0f21ae77a4eedad9e |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:c99a47b850832ec9ceb1cb5fac6b4e46e745f59c2019934d25c2cfe8f2b36b10  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:54f43396b246dc5ddfe0c2d1d2458f4a311508fe07dcde0e517955873dd7296a |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:212aded9c810bb48979b300156382c1384a6145f867f02f691d70946991746f0 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:c99a47b850832ec9ceb1cb5fac6b4e46e745f59c2019934d25c2cfe8f2b36b10 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:a03a306209f9ae8d370a0f7c9459e00ae83d4d22ae483b4f81df97308958e127 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:212aded9c810bb48979b300156382c1384a6145f867f02f691d70946991746f0 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:af4de6d02421a6dfaebf071f726152cd09e53a08d9955a0b680406d323a10a12 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:ed88b3873a0af645f2404bb0423bdf27a37fdd3c80bbac2464bf1952d40aa46b |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:18058dc1e5ee3febb327a13d846fa80533de365788e3e03ed00e358ef45581ff |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:907b1187b1e47e17a1392d38856731ced3da418645b023062e3cf292e6ee99eb
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:2b97c8539b2fe8d7d6a276f839613fb6bfa57e902723d76ca998628693e4475e
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:464598f26343bb776752aa0bd6142e2d40c6b7384875b0e0f21ae77a4eedad9e
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:00c6c0571d6b13176522ac357b72910af31f6cd698bca54ff90ad9e8ccffa1e3
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:18058dc1e5ee3febb327a13d846fa80533de365788e3e03ed00e358ef45581ff
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:ed88b3873a0af645f2404bb0423bdf27a37fdd3c80bbac2464bf1952d40aa46b
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:54f43396b246dc5ddfe0c2d1d2458f4a311508fe07dcde0e517955873dd7296a
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:c99a47b850832ec9ceb1cb5fac6b4e46e745f59c2019934d25c2cfe8f2b36b10
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:212aded9c810bb48979b300156382c1384a6145f867f02f691d70946991746f0
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:a03a306209f9ae8d370a0f7c9459e00ae83d4d22ae483b4f81df97308958e127
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:dac18aafbd462e766ae4f1806284bf9c48a5496e65c52fe1f16877655a283b80
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:b98a23cabda8c19bb4e488f46487b9c17a319e12ca00d833d7de139ff373b8b9
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:af4de6d02421a6dfaebf071f726152cd09e53a08d9955a0b680406d323a10a12
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
