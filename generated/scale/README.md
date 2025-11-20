
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:6dcb6ca5430deea044cfd029df4a9f0576586e824af07d9c61f4630ee4798e11 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:2c2e9c630a45da80321bbf1b63e9152e0cb7cc14390ee3879fd736e0a6974464 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:798559d9dfabfbd2cca1224fde8f6b0cbc4c96fd9d01212ea07bfdb4e40c8818 |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:51dc287dd9ae2f8dcb60c1678fe8b535bb72e29faad24108d55b7cfe62362777 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:51dc287dd9ae2f8dcb60c1678fe8b535bb72e29faad24108d55b7cfe62362777 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:539f31bb5691b636f2a7236b3fa617ba38e7ed35b7a3b1e71de5e84fd16f4d26 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:07ae36c1a8539aee091cff19261aa14a9d220e6994132a14d2d8c537d596f9ec |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:3b48c09f3641c10c63378a2dda806673fe7ea9c43774112f67bd8f8bd4e53b93  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:57ea64cdd612aef7a5f01dfbd41677092c0f565c35ef7e5394e50799dc3796e1 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:c77c0b3c6f7373136b581dabf2f57899c8a742d1cb4501d739af95cba151a438 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:3b48c09f3641c10c63378a2dda806673fe7ea9c43774112f67bd8f8bd4e53b93 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:ad1e25622e325f4aa3000e680bd747bea50a22b65a8472cbc20640b730c86fa4 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:c77c0b3c6f7373136b581dabf2f57899c8a742d1cb4501d739af95cba151a438 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:711f9fc45969639da712b0823139549cdbedead0be9453c4243e1a873e7737f1 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:b3b91b2f6729ecb3544b6b9fc539e2abbe425dfe497ce88deba7deed55305c7c |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:6dcb6ca5430deea044cfd029df4a9f0576586e824af07d9c61f4630ee4798e11
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:539f31bb5691b636f2a7236b3fa617ba38e7ed35b7a3b1e71de5e84fd16f4d26
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:07ae36c1a8539aee091cff19261aa14a9d220e6994132a14d2d8c537d596f9ec
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:51dc287dd9ae2f8dcb60c1678fe8b535bb72e29faad24108d55b7cfe62362777
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:b3b91b2f6729ecb3544b6b9fc539e2abbe425dfe497ce88deba7deed55305c7c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:57ea64cdd612aef7a5f01dfbd41677092c0f565c35ef7e5394e50799dc3796e1
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:3b48c09f3641c10c63378a2dda806673fe7ea9c43774112f67bd8f8bd4e53b93
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:c77c0b3c6f7373136b581dabf2f57899c8a742d1cb4501d739af95cba151a438
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:ad1e25622e325f4aa3000e680bd747bea50a22b65a8472cbc20640b730c86fa4
cp.icr.io/cp/gpfs/postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:798559d9dfabfbd2cca1224fde8f6b0cbc4c96fd9d01212ea07bfdb4e40c8818
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:2c2e9c630a45da80321bbf1b63e9152e0cb7cc14390ee3879fd736e0a6974464
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:711f9fc45969639da712b0823139549cdbedead0be9453c4243e1a873e7737f1
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
