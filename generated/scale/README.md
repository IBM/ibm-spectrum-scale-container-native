
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:d2f9ebc3bb196ad85b931f2dabdce13aed2e6598227b8fc2434d6df9f840f696 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:8d74a489683d33a2e21d2b00b774d08b51861213fcd0a93ad93a1a1658595439 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:4ce047b7b8f81652fd6c2c0a6682d92c08b5e99e1f31dcdde196e01267f58cc9 |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:8bd2d8d1663d5a709327561d92e962ed1e6fb4925df9925701a637cadc22be2b |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:8bd2d8d1663d5a709327561d92e962ed1e6fb4925df9925701a637cadc22be2b |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:72c607d9288093b3e18fda25bb9ae608c931343254987a2b3bfc7c647afeea5c |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:e287f6538f619dd1b06884fc7c3ca957366b8e365782539addb83bfa13a92be1 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:ef767949384ffdf4f2067496051961a7b2c75e52d9255991ce0152072bfb9d2d  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:179fd0f462c15f303c7a006b1a8ad71f01cd4215bcac99ac46722e37a56dba93 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:9543dfe369c3d1d4bd93f7c7743f990ae652e9bc2256a0ba6ed1d03e6924afd0 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:ef767949384ffdf4f2067496051961a7b2c75e52d9255991ce0152072bfb9d2d |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:f4c3d343e92a9931830b2693bc274136a14f6f497e7da92c199a957b9c0a0c7a |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:9543dfe369c3d1d4bd93f7c7743f990ae652e9bc2256a0ba6ed1d03e6924afd0 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:4856f2904c1893e8893f6d8e6775c23fe0871f0547c5d24984d70bbbbb7b3580 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:b05cf7a8f6e1be3aa576f237075757fb318c9d3174f54410dbc17365176ce121 |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:d2f9ebc3bb196ad85b931f2dabdce13aed2e6598227b8fc2434d6df9f840f696
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:72c607d9288093b3e18fda25bb9ae608c931343254987a2b3bfc7c647afeea5c
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:e287f6538f619dd1b06884fc7c3ca957366b8e365782539addb83bfa13a92be1
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:8bd2d8d1663d5a709327561d92e962ed1e6fb4925df9925701a637cadc22be2b
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:b05cf7a8f6e1be3aa576f237075757fb318c9d3174f54410dbc17365176ce121
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:179fd0f462c15f303c7a006b1a8ad71f01cd4215bcac99ac46722e37a56dba93
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:ef767949384ffdf4f2067496051961a7b2c75e52d9255991ce0152072bfb9d2d
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:9543dfe369c3d1d4bd93f7c7743f990ae652e9bc2256a0ba6ed1d03e6924afd0
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:f4c3d343e92a9931830b2693bc274136a14f6f497e7da92c199a957b9c0a0c7a
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmsensors@sha256:c9270e17334eba8fd77733282bb78866fa7266e87d86bcb19146a116d4e83483
cp.icr.io/cp/gpfs/postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:4ce047b7b8f81652fd6c2c0a6682d92c08b5e99e1f31dcdde196e01267f58cc9
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:8d74a489683d33a2e21d2b00b774d08b51861213fcd0a93ad93a1a1658595439
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:4856f2904c1893e8893f6d8e6775c23fe0871f0547c5d24984d70bbbbb7b3580
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
