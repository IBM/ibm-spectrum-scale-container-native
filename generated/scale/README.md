
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:7e4fd0ffb813d034ec9b553d002b78c60e3a8f2550681613ce9c954d6e43109f |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:142bbc39ef762240505a7cba38a7ae1564876c50f071abc125f8e6da0632ef77 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:367d038014e9f772e310eb6baf36590d20e9347261fec2cba97636739828b81e |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:e4b7ecadb723f39217bfda439ae58fa537a913552cbfa0c71247e6c0224c6d62 |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:e4b7ecadb723f39217bfda439ae58fa537a913552cbfa0c71247e6c0224c6d62 |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:9eb90c13c04f0d0c202be53a3c471b8a90d322b36a4ba488029b0f01ed1752dc |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:00ffcf508c1212841eb9915c66e7fa723ca3a7b95f23c933efbad3f3a84ce273 |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:ac61c96b93894b9169221e87718733354dd3765dd4a62b275893c7ff0d876869  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:0f8d7f433a16c0d8254d5604387f80f830914c74fdff05ddd5a7485b559f96a4 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:59a92d0ea321b917de5e9114d39f891d1659357c12b5317bb6282f0c9cd8b226 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:ac61c96b93894b9169221e87718733354dd3765dd4a62b275893c7ff0d876869 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:cb76b64eaca21d562717ade6d04b92812ac4f8dca006c3b61db80bbc5412f3dd |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:59a92d0ea321b917de5e9114d39f891d1659357c12b5317bb6282f0c9cd8b226 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:4627f333f4b5e6d692c9dd7a1868c00912abed27155dcfd0915184ba1257662e |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:879f0dd5c00590698be68f53005a7e538c6c6cca523854368640435df794d950 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:9294e154a26e9f4f0e725b282a1092678b21bb7043709b0fd2fe9131e10786ce |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:7e4fd0ffb813d034ec9b553d002b78c60e3a8f2550681613ce9c954d6e43109f
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:9eb90c13c04f0d0c202be53a3c471b8a90d322b36a4ba488029b0f01ed1752dc
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:00ffcf508c1212841eb9915c66e7fa723ca3a7b95f23c933efbad3f3a84ce273
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:e4b7ecadb723f39217bfda439ae58fa537a913552cbfa0c71247e6c0224c6d62
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:879f0dd5c00590698be68f53005a7e538c6c6cca523854368640435df794d950
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:4627f333f4b5e6d692c9dd7a1868c00912abed27155dcfd0915184ba1257662e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:0f8d7f433a16c0d8254d5604387f80f830914c74fdff05ddd5a7485b559f96a4
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:59a92d0ea321b917de5e9114d39f891d1659357c12b5317bb6282f0c9cd8b226
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:cb76b64eaca21d562717ade6d04b92812ac4f8dca006c3b61db80bbc5412f3dd
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmsensors@sha256:5e6073fdedd133215936cf3b17c2508b09a01049b5c027a267af6349f43ae318
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:ac61c96b93894b9169221e87718733354dd3765dd4a62b275893c7ff0d876869
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:367d038014e9f772e310eb6baf36590d20e9347261fec2cba97636739828b81e
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:142bbc39ef762240505a7cba38a7ae1564876c50f071abc125f8e6da0632ef77
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:9294e154a26e9f4f0e725b282a1092678b21bb7043709b0fd2fe9131e10786ce
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
```
