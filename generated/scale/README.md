
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:ec39d48e72c086961ad7b65384f09af137977cbb4b8b218aa7d572c3c7501046 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:a247e6bde9a851d80b671b01150dbe7267129b4650cf50cfef046ac28b2d9c8d |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:c9b091bd73585a1361689bbb11a78f76883185f7a76cc872bb77c0a4c9ab2b8c |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:a5018ab3a65f6d35cc285bb5faf0fb5c94ff2eb63839fa1cd790da51e730cde7 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:a5018ab3a65f6d35cc285bb5faf0fb5c94ff2eb63839fa1cd790da51e730cde7 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:7176d27df707a7601d8ee6cc70cfda3b7e37aef788826e6299a942a6995ceb4d |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:128ac106637fdf64cfb6cbc0fa3a5d18ab698509118a20ff93e88b091139fc0c |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:31a5c265df2a3183885e601369435f986baa6c8375ed7d6b827422b464015389  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:324e700c049ee9eb5239c6baada0eeb1b9389877fcb0f3366e596d294d5c82e9 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:e32160671466a3794364c099712cf69761530d3728b548a5b951f6f6a9d3b541 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:31a5c265df2a3183885e601369435f986baa6c8375ed7d6b827422b464015389 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:2398d15d59a0a66603a510d9196d5a30517787c89fe347b2507b06d343f1c2cd |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:e32160671466a3794364c099712cf69761530d3728b548a5b951f6f6a9d3b541 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:35ffde86b9805b83862a07acff838d086006cd3277424c8630de4697218a31e6 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:b45261f1b673e4f933d512ce7ac31b72da1b4fa1229809181bf6f089cadbd6ed |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:18058dc1e5ee3febb327a13d846fa80533de365788e3e03ed00e358ef45581ff |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:ec39d48e72c086961ad7b65384f09af137977cbb4b8b218aa7d572c3c7501046
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:7176d27df707a7601d8ee6cc70cfda3b7e37aef788826e6299a942a6995ceb4d
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:128ac106637fdf64cfb6cbc0fa3a5d18ab698509118a20ff93e88b091139fc0c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:a5018ab3a65f6d35cc285bb5faf0fb5c94ff2eb63839fa1cd790da51e730cde7
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:18058dc1e5ee3febb327a13d846fa80533de365788e3e03ed00e358ef45581ff
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:b45261f1b673e4f933d512ce7ac31b72da1b4fa1229809181bf6f089cadbd6ed
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:324e700c049ee9eb5239c6baada0eeb1b9389877fcb0f3366e596d294d5c82e9
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:31a5c265df2a3183885e601369435f986baa6c8375ed7d6b827422b464015389
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:e32160671466a3794364c099712cf69761530d3728b548a5b951f6f6a9d3b541
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:2398d15d59a0a66603a510d9196d5a30517787c89fe347b2507b06d343f1c2cd
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:c9b091bd73585a1361689bbb11a78f76883185f7a76cc872bb77c0a4c9ab2b8c
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:a247e6bde9a851d80b671b01150dbe7267129b4650cf50cfef046ac28b2d9c8d
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:35ffde86b9805b83862a07acff838d086006cd3277424c8630de4697218a31e6
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
