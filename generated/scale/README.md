
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:731987d4b3f39ca78017d227b5fc6fa9ed5db95567dde436fda7b86da8d7b8ae
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:7ad6859d4a6f59e638046ed5d99cba7f5da5934ae4b2e519769d635a2cc5f884 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:efc68a9efa10884325e075affb207875cc199b2ad8950eaad772456573ff2595 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:efc68a9efa10884325e075affb207875cc199b2ad8950eaad772456573ff2595 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:6c146ab5ce9a9e4dd89fdb17c5797f76cef659e8c96cae48e640d9e0d9bf181a |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:c4789f677a9d3c66484671f7227fa130c356ae416faf5a61f2cd31a250b122f7 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:e4731ab55d571d722abfaa34d8efa29a4059430a2ef1096e51a80cdb0bbdd496  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:c2813671dac5715a90281b5d509539a691a0afd7a5b8a7b0b618b32e38207609 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:de4d18a1fb0182023d9ba827b2ed3258248522e7422940b3fb0d071fc0a89ac1 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:aa6eb304ddb6dd26df23d05db4e5cb05af8951cda3e0dc57731b771e0ef4ab29 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:e4731ab55d571d722abfaa34d8efa29a4059430a2ef1096e51a80cdb0bbdd496 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:0d91c39b45ced31f6c05c021a104603e0f264d25877e7639f98044cfd8185aa2 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:de4d18a1fb0182023d9ba827b2ed3258248522e7422940b3fb0d071fc0a89ac1 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:da081c27e8a6d91f36042c1942362d0515ced8d06e18c11b8f893e58c4d6d797  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:b74b05b39501565022883fc128002b4cb857a7bb6c858606bcb3fdedba0b0b80 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:6be9f63ca4caa6c46aae55aa372500949d8a21473d72f819da1f746076b32d4e |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:c4cc074199c045dd73ab85f28897e2a32f4d6f38ffdba4f3b13b8007ccbd3570 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:ab482308a4921e28a6df09a16ab99a457e9af9641ff44fb1be1a690d07ce8b70 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:589e525cddef6d768e68da1f0bc9ffd0a24bf3add3dd010648eb7189976fde79 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:512b2bcc5300b7356c423ddbae0f3413c46fc17c2b5c73c057019ddd34ef69a5 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:cd472a0b796eeee284963df4abc78a54bac6b7cd2ca88fa31ec699b14d823bc6 |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:ffb912e9c0e80a87c6733df0df63e05b499ae575e90210db0d53e344bf4ec35c |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:731987d4b3f39ca78017d227b5fc6fa9ed5db95567dde436fda7b86da8d7b8ae
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:6c146ab5ce9a9e4dd89fdb17c5797f76cef659e8c96cae48e640d9e0d9bf181a
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:c4789f677a9d3c66484671f7227fa130c356ae416faf5a61f2cd31a250b122f7
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:efc68a9efa10884325e075affb207875cc199b2ad8950eaad772456573ff2595
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:ffb912e9c0e80a87c6733df0df63e05b499ae575e90210db0d53e344bf4ec35c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:cd472a0b796eeee284963df4abc78a54bac6b7cd2ca88fa31ec699b14d823bc6
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:c2813671dac5715a90281b5d509539a691a0afd7a5b8a7b0b618b32e38207609
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:e4731ab55d571d722abfaa34d8efa29a4059430a2ef1096e51a80cdb0bbdd496
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:de4d18a1fb0182023d9ba827b2ed3258248522e7422940b3fb0d071fc0a89ac1
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:0d91c39b45ced31f6c05c021a104603e0f264d25877e7639f98044cfd8185aa2
cp.icr.io/cp/gpfs/postgres@sha256:aa6eb304ddb6dd26df23d05db4e5cb05af8951cda3e0dc57731b771e0ef4ab29
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:7ad6859d4a6f59e638046ed5d99cba7f5da5934ae4b2e519769d635a2cc5f884
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:b74b05b39501565022883fc128002b4cb857a7bb6c858606bcb3fdedba0b0b80
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:ab482308a4921e28a6df09a16ab99a457e9af9641ff44fb1be1a690d07ce8b70
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:6be9f63ca4caa6c46aae55aa372500949d8a21473d72f819da1f746076b32d4e
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:589e525cddef6d768e68da1f0bc9ffd0a24bf3add3dd010648eb7189976fde79
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:da081c27e8a6d91f36042c1942362d0515ced8d06e18c11b8f893e58c4d6d797
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:512b2bcc5300b7356c423ddbae0f3413c46fc17c2b5c73c057019ddd34ef69a5
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:c4cc074199c045dd73ab85f28897e2a32f4d6f38ffdba4f3b13b8007ccbd3570
```
