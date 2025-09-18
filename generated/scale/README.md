
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:8b1793ef7c7858cdcd1a85ecffbbec9e981615dba8a8c11e9edc3f1035e88494 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:3f358e4d2895867198ee114b90ce5923325115ef75a2b49751280901423e3464 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:4364bae5e90691466e1c01780359ca152f8cfe8e118d4c1ec0f929ab641c64df |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:63fb2d337983f935652adb0e6582bc1adf68c1af52b5ff071430ae200d2a8759 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:63fb2d337983f935652adb0e6582bc1adf68c1af52b5ff071430ae200d2a8759 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:76e25fadfd36279b440adac5a96f30060762a1239ad9990da907931200a6788a |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:7c1bde7f7b195cf16f418a8ca4935c9b8cb615deb7abd5ce6261369dc66efba8 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:43ff86e15a214223fbe8d9ebfdbb4b3a4affd76dc37febeae665cf0c8e69e2d8  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:e28be0799e62625504c0a7514e22f0946c943b39acebee63970f002112c87867 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:58035894d2f16b3f198eaab41a4f4031c3c6afea4efa46a857de3fdc59a858a3 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:43ff86e15a214223fbe8d9ebfdbb4b3a4affd76dc37febeae665cf0c8e69e2d8 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:f64e2e6f0faf709093ec535b1c790ada8fd5ff88c96e7e793160271d55a53421 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:58035894d2f16b3f198eaab41a4f4031c3c6afea4efa46a857de3fdc59a858a3 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:9fbd6cb9b434faa7431e0b7cb8b7423baeb0d9cea4db365b76af60b35d460054 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:ce0de4057f5980183ca82f67d241d50e5c63b7b0c43bceb1ca847525f9fd58c5 |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:8b1793ef7c7858cdcd1a85ecffbbec9e981615dba8a8c11e9edc3f1035e88494
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:76e25fadfd36279b440adac5a96f30060762a1239ad9990da907931200a6788a
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:7c1bde7f7b195cf16f418a8ca4935c9b8cb615deb7abd5ce6261369dc66efba8
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:63fb2d337983f935652adb0e6582bc1adf68c1af52b5ff071430ae200d2a8759
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:6a317b23fee629c0b07eb95d34ab7593bb38d41bffc5d1cd4cb2870539c66cd4
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:ce0de4057f5980183ca82f67d241d50e5c63b7b0c43bceb1ca847525f9fd58c5
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:e28be0799e62625504c0a7514e22f0946c943b39acebee63970f002112c87867
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:43ff86e15a214223fbe8d9ebfdbb4b3a4affd76dc37febeae665cf0c8e69e2d8
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:58035894d2f16b3f198eaab41a4f4031c3c6afea4efa46a857de3fdc59a858a3
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:f64e2e6f0faf709093ec535b1c790ada8fd5ff88c96e7e793160271d55a53421
cp.icr.io/cp/gpfs/postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:4364bae5e90691466e1c01780359ca152f8cfe8e118d4c1ec0f929ab641c64df
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:3f358e4d2895867198ee114b90ce5923325115ef75a2b49751280901423e3464
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:69888dba58159c8bc0d7c092b9fb97900c9ca8710d088b0b7ea7bd9052df86f6
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:d7138bcc3aa5f267403d45ad4292c95397e421ea17a0035888850f424c7de25d
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:d5e46da8aff7d73d6f00c761dae94472bcda6e78f4f17b3802dc89d44de0111b
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:8ddd178ba5d08973f1607f9b84619b58320948de494b31c9d7cd5375b316d6d4
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:5f4bb469fec51147ce157329dab598c758da1b018bad6dad26f0ff469326d769
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:9fbd6cb9b434faa7431e0b7cb8b7423baeb0d9cea4db365b76af60b35d460054
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:2c5f9dc4ea5ac5509d93c664ae7982d4ecdec40ca7b0638c24e5b16243b8360f
```
