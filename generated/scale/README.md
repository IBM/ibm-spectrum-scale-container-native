
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:393cf5b2e1e6a5834277fc309f8c2a5c0febc8be4fa3503b4e5144bb47981e6a |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:4cffa1292565ed746fb5e9e2741df17552a63b855295f24330ceeb9bd7c03517 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:76749a094007d82ac7e7dc9544f4b62df18c764f183540cdff1e635f53bf6b96 |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:3648c55e87844fba8c0fbc42c98bebf7e9e9474325b9a479a170ba1b46818f0a |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:3648c55e87844fba8c0fbc42c98bebf7e9e9474325b9a479a170ba1b46818f0a |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:c544d7c1b2eeca8367bc97a4f882e99c8773de765a365c90d5e79bee00703cec |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:ef9b26a2ab68c8b4f71d5a77080ec440d691766f36a34b22d033b0c4c1dae8c5 |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:b87097994ed62fbf1de70bc75debe8dacf3ea6e00dd577d74503ef66452c59d6  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:7dbcc1cf67a1cf766cb15cce16f12cfa945eb7c97a83bd49859aa78754853fc8 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:b2ba274826407002fe2e5478ad8c8b8e60eb7249ef69c16ae29dd6efca3d100b |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:b87097994ed62fbf1de70bc75debe8dacf3ea6e00dd577d74503ef66452c59d6 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:bbbf37dda4858b77b6c77f5b342de000cea32e538183041642578c33ec7fc058 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:b2ba274826407002fe2e5478ad8c8b8e60eb7249ef69c16ae29dd6efca3d100b |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:ea6fa2c9fcfb20316a86255c51132132b810788a37b4e543d1577419786198ef |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:879f0dd5c00590698be68f53005a7e538c6c6cca523854368640435df794d950 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:92c6c50ebe8c8845b202680a5b40f94e52a34433c2e12e0f5747032982e711e7 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:393cf5b2e1e6a5834277fc309f8c2a5c0febc8be4fa3503b4e5144bb47981e6a
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:c544d7c1b2eeca8367bc97a4f882e99c8773de765a365c90d5e79bee00703cec
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:ef9b26a2ab68c8b4f71d5a77080ec440d691766f36a34b22d033b0c4c1dae8c5
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:3648c55e87844fba8c0fbc42c98bebf7e9e9474325b9a479a170ba1b46818f0a
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:879f0dd5c00590698be68f53005a7e538c6c6cca523854368640435df794d950
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:ea6fa2c9fcfb20316a86255c51132132b810788a37b4e543d1577419786198ef
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:7dbcc1cf67a1cf766cb15cce16f12cfa945eb7c97a83bd49859aa78754853fc8
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:b2ba274826407002fe2e5478ad8c8b8e60eb7249ef69c16ae29dd6efca3d100b
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:bbbf37dda4858b77b6c77f5b342de000cea32e538183041642578c33ec7fc058
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmsensors@sha256:f1fb6a9381b1dcab36c281febc6f3d321248908d90ad7ed3b960ae37506ee3a1
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:b87097994ed62fbf1de70bc75debe8dacf3ea6e00dd577d74503ef66452c59d6
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:76749a094007d82ac7e7dc9544f4b62df18c764f183540cdff1e635f53bf6b96
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:4cffa1292565ed746fb5e9e2741df17552a63b855295f24330ceeb9bd7c03517
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:92c6c50ebe8c8845b202680a5b40f94e52a34433c2e12e0f5747032982e711e7
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
```
