
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:f05458bc60d84522cf9ac4386151ed05454273ed9c8078db743bb406891ffde8 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:c5ab8375e746233fe3370af25c4b6431742e95d04d042b4b2587002c8c3e71a6 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:961dae6fed4b8b2ef8e4e20db2bac41c79ff5a302e50f7f552dfb4b61ea1d08e |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:aeba255fe8a865ebf57618fcb490961854526008d86e31cd14f4495768071599 |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:aeba255fe8a865ebf57618fcb490961854526008d86e31cd14f4495768071599 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:2a52918950b00e99659950d4aec06141f447a0f258af78a96181d47fbcdd7594 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:3b151f02b65f8afcc5eb6bfe4a301efdf57a07f1e0d1733207c60ced583f9f9c |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:bc552efb4966aaa44b02532be3168ac1ff18e2af299d0fe89502a1d9fabafbc5  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:78216ac2a8157753bd70f273f5e696479538007f43312bacd8e7f8e30f146276 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:9d340ff16b39373ded4b6baea7210d5daeb2a7ce91d65447ad156e0c9dc2f4cd |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:bc552efb4966aaa44b02532be3168ac1ff18e2af299d0fe89502a1d9fabafbc5 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:bc7c25bd407f0abbd980cb59fbc2353ab41fb2fffb3f8d00aac9b000584cd1ba |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:9d340ff16b39373ded4b6baea7210d5daeb2a7ce91d65447ad156e0c9dc2f4cd |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:1a29ab1e4ecdc33a84062cec757620d9787c28b28793202c5b78ae097c3dee27  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:d69cc72025f7c40dae112ff989e920a3331583497c8dfb1600c5ae0e37184a29 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:de79c8bbc271622eb94d2ee8689f189ea7c1cb6adac260a421980fe5eed66708 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:c53535af8a7f7e3164609838c4b191b42b2d81238d75c1b2a2b582ada62a9780 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:4c148bbdf883153bc72d321be4dc55c33774a6d98b2b3e0c2da6ae389149a9b7 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:fb25463d85c1a81555e481118b24c30d337397a9719547a02d3a408bb645ae0f |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:cb7133b83cf96ca1c6c697a48de3faf57197d2a46225102d451cc7c7217bec30 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:f05458bc60d84522cf9ac4386151ed05454273ed9c8078db743bb406891ffde8
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:2a52918950b00e99659950d4aec06141f447a0f258af78a96181d47fbcdd7594
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:3b151f02b65f8afcc5eb6bfe4a301efdf57a07f1e0d1733207c60ced583f9f9c
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:aeba255fe8a865ebf57618fcb490961854526008d86e31cd14f4495768071599
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:bc7c25bd407f0abbd980cb59fbc2353ab41fb2fffb3f8d00aac9b000584cd1ba
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:9d340ff16b39373ded4b6baea7210d5daeb2a7ce91d65447ad156e0c9dc2f4cd
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:78216ac2a8157753bd70f273f5e696479538007f43312bacd8e7f8e30f146276
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:cb7133b83cf96ca1c6c697a48de3faf57197d2a46225102d451cc7c7217bec30
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:961dae6fed4b8b2ef8e4e20db2bac41c79ff5a302e50f7f552dfb4b61ea1d08e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:bc552efb4966aaa44b02532be3168ac1ff18e2af299d0fe89502a1d9fabafbc5
cp.icr.io/cp/spectrum/scale/postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:c5ab8375e746233fe3370af25c4b6431742e95d04d042b4b2587002c8c3e71a6
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:fb25463d85c1a81555e481118b24c30d337397a9719547a02d3a408bb645ae0f
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:1a29ab1e4ecdc33a84062cec757620d9787c28b28793202c5b78ae097c3dee27
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:de79c8bbc271622eb94d2ee8689f189ea7c1cb6adac260a421980fe5eed66708
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:c53535af8a7f7e3164609838c4b191b42b2d81238d75c1b2a2b582ada62a9780
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:d69cc72025f7c40dae112ff989e920a3331583497c8dfb1600c5ae0e37184a29
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:4c148bbdf883153bc72d321be4dc55c33774a6d98b2b3e0c2da6ae389149a9b7
```
