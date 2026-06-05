
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:5e2095f878f45b561e17fc00725d6ca69653d12f7693d295b0a53a40046f1a45
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:39d5a03dcc657ce704299767e09408e52be040edf11d8a2cf4b72864178e4535 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:1775f4d2c51ae9bef6d0d129c79efcfefb4d6d4008445d57b852d4c4397b2fe2 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:1775f4d2c51ae9bef6d0d129c79efcfefb4d6d4008445d57b852d4c4397b2fe2 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:9f310dc6111fdc2b32f3a8c0d1670e407716706cf92e60910ddf3816009632ab |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:3651a79cfd42e67416995af3442b667beef09c9c1417e406b7be20cb63497ddf |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:16754a6b3e1eaac73a3df6d6ded01d31e0f5d0cc75dc6f30d1cb8043d2dc0685  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:fd85ae58cfdf4ef48b300f542967a0b2e626ff4015af86a5f31e648b76d11160 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:a15797ec26b5e6b54de4396ed4fdb9303169908c04337694ff2d2f2e9372df87 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:aa6eb304ddb6dd26df23d05db4e5cb05af8951cda3e0dc57731b771e0ef4ab29 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:16754a6b3e1eaac73a3df6d6ded01d31e0f5d0cc75dc6f30d1cb8043d2dc0685 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:10dd10e7ab9c32d36b31924c266671573c48fe1fd4c43cb1a6d89d7644482a4c |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:a15797ec26b5e6b54de4396ed4fdb9303169908c04337694ff2d2f2e9372df87 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:da081c27e8a6d91f36042c1942362d0515ced8d06e18c11b8f893e58c4d6d797  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:b74b05b39501565022883fc128002b4cb857a7bb6c858606bcb3fdedba0b0b80 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:6be9f63ca4caa6c46aae55aa372500949d8a21473d72f819da1f746076b32d4e |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:c4cc074199c045dd73ab85f28897e2a32f4d6f38ffdba4f3b13b8007ccbd3570 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:ab482308a4921e28a6df09a16ab99a457e9af9641ff44fb1be1a690d07ce8b70 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:589e525cddef6d768e68da1f0bc9ffd0a24bf3add3dd010648eb7189976fde79 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:35c2c45c0a8f6504cf50dda57fd0c827244e822e02febf449a37630fc6d01b9d |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:3843a5db15d214355d7c80751b7ab771cbaef9be025eea04745386d9210914e5 |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:781db6ee6019ae2468b57f48abc17033ccfcdb88beb555b2797ee4fe32a2731b |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:5e2095f878f45b561e17fc00725d6ca69653d12f7693d295b0a53a40046f1a45
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:9f310dc6111fdc2b32f3a8c0d1670e407716706cf92e60910ddf3816009632ab
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:3651a79cfd42e67416995af3442b667beef09c9c1417e406b7be20cb63497ddf
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:1775f4d2c51ae9bef6d0d129c79efcfefb4d6d4008445d57b852d4c4397b2fe2
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:781db6ee6019ae2468b57f48abc17033ccfcdb88beb555b2797ee4fe32a2731b
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:3843a5db15d214355d7c80751b7ab771cbaef9be025eea04745386d9210914e5
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:fd85ae58cfdf4ef48b300f542967a0b2e626ff4015af86a5f31e648b76d11160
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:16754a6b3e1eaac73a3df6d6ded01d31e0f5d0cc75dc6f30d1cb8043d2dc0685
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:a15797ec26b5e6b54de4396ed4fdb9303169908c04337694ff2d2f2e9372df87
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:10dd10e7ab9c32d36b31924c266671573c48fe1fd4c43cb1a6d89d7644482a4c
cp.icr.io/cp/gpfs/postgres@sha256:aa6eb304ddb6dd26df23d05db4e5cb05af8951cda3e0dc57731b771e0ef4ab29
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:39d5a03dcc657ce704299767e09408e52be040edf11d8a2cf4b72864178e4535
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:b74b05b39501565022883fc128002b4cb857a7bb6c858606bcb3fdedba0b0b80
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:ab482308a4921e28a6df09a16ab99a457e9af9641ff44fb1be1a690d07ce8b70
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:6be9f63ca4caa6c46aae55aa372500949d8a21473d72f819da1f746076b32d4e
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:589e525cddef6d768e68da1f0bc9ffd0a24bf3add3dd010648eb7189976fde79
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:da081c27e8a6d91f36042c1942362d0515ced8d06e18c11b8f893e58c4d6d797
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:35c2c45c0a8f6504cf50dda57fd0c827244e822e02febf449a37630fc6d01b9d
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:c4cc074199c045dd73ab85f28897e2a32f4d6f38ffdba4f3b13b8007ccbd3570
```
