
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:3979c40e5d70905aa10ec321c69dfbe7b1cedaf884483b7321bf916c386b6e0b |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:a16f6f3e81f83b6d8db555d88ae15a0a0c2b06427e573b0393c45f59fb1d446c |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:8bd88e708af5d0001c3101a2c97ca3cffcf0fa8c259acbc9c1c160e89e32981c |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:6caa1873e84cb5ed13ecbe8a58a4bbfc583aba8638c84fbaab216c0b8a80acd6 |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:6caa1873e84cb5ed13ecbe8a58a4bbfc583aba8638c84fbaab216c0b8a80acd6 |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:d0ee7b46a3de6a8db7c455f2f953f5fdc35e98b4846179184f67d1488f107f71 |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:2099d2b85f76ceb63975504f71ecf74c91f8850123c6fcda30555a11b4c59191 |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:8d905a93f1392d4a8f7fb906bd49bf540290674b28d82de3536bb4d0898bf9d7  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:023bf59d37178031fd65164257c4601cd004c005e8881cf49152414a8b6c0343 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:79ef7f8df331d8e00ea3b112ad9c3bb6c0888ee7b064c5e4bd72b5326d5e3951 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:8d905a93f1392d4a8f7fb906bd49bf540290674b28d82de3536bb4d0898bf9d7 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:00d3b00f219175a748504b5393dccc2fdfc05a870d328109ac020200e7ce4f8f |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:79ef7f8df331d8e00ea3b112ad9c3bb6c0888ee7b064c5e4bd72b5326d5e3951 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:d3c17cfe888230dea86a0ddab9d90a99de82d7892bc2ac1b4ce21b90738f9b15 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:879f0dd5c00590698be68f53005a7e538c6c6cca523854368640435df794d950 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:fd707136a9c59b9bfc264b15f3df0248b5770e0da3ea3016b668d04ecaac39d5 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:3979c40e5d70905aa10ec321c69dfbe7b1cedaf884483b7321bf916c386b6e0b
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:d0ee7b46a3de6a8db7c455f2f953f5fdc35e98b4846179184f67d1488f107f71
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:2099d2b85f76ceb63975504f71ecf74c91f8850123c6fcda30555a11b4c59191
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:6caa1873e84cb5ed13ecbe8a58a4bbfc583aba8638c84fbaab216c0b8a80acd6
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:879f0dd5c00590698be68f53005a7e538c6c6cca523854368640435df794d950
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:d3c17cfe888230dea86a0ddab9d90a99de82d7892bc2ac1b4ce21b90738f9b15
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:023bf59d37178031fd65164257c4601cd004c005e8881cf49152414a8b6c0343
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:79ef7f8df331d8e00ea3b112ad9c3bb6c0888ee7b064c5e4bd72b5326d5e3951
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:00d3b00f219175a748504b5393dccc2fdfc05a870d328109ac020200e7ce4f8f
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmsensors@sha256:8ebdad85e4e43f1db5027fa8042ec05dbab830c90ffeb76f92dce37e02632d37
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:8d905a93f1392d4a8f7fb906bd49bf540290674b28d82de3536bb4d0898bf9d7
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:8bd88e708af5d0001c3101a2c97ca3cffcf0fa8c259acbc9c1c160e89e32981c
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:a16f6f3e81f83b6d8db555d88ae15a0a0c2b06427e573b0393c45f59fb1d446c
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:fd707136a9c59b9bfc264b15f3df0248b5770e0da3ea3016b668d04ecaac39d5
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
```
