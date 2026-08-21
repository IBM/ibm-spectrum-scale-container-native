
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:85d026352226e82d36ea400d8e5266afd1dbc0d4de1200d25d3d4012b4e4af41
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:5c9bf563902de42a053c8fc33e9e1f8c0b033fb606ea2f2c0ec012c22f400566 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:92231b42ede5f888c9c98c7f8ab9c276d59124a2c41030b7b8739f2bf25edec8 |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:92231b42ede5f888c9c98c7f8ab9c276d59124a2c41030b7b8739f2bf25edec8 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:3b1ca9e89f557f32e43e76529de8da986ee003cc0f4a54a7365035a6170e1f94 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:1f3bfd60724100c42a168bed67a8fe8bdc94101d93d0883cded1d3849b1054f6 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:14ace17c2fdc55018dab61c26d1023f8d9794a9b6b9e6d38be339a36dfc732fa  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:87260cf83b207019a7dbfe2d2f82c5f230a1f156a026a5250a97abfc1de55e00 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:7eaa8a0b20cd47c905e3a1444723c0d76c2b156105692af536bfa2e2d1b58b34 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:14ace17c2fdc55018dab61c26d1023f8d9794a9b6b9e6d38be339a36dfc732fa |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:a25b5384e0d3a6f31ca1047e32332a5b58267cf54a0794b63fb34757e46d2ecb |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:7eaa8a0b20cd47c905e3a1444723c0d76c2b156105692af536bfa2e2d1b58b34 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:dd589aa2abd408d2e9c8f6a0b001db27802f1c3175a95c54f7c2d4993f6ae8d4 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:bf8189141c40693c270260e5713202d850ff00db4404912230c4a9201a80aa8c |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:d5f4690898d9468a22d92f6da530cd28966dffc4e8519de89236954a3815dd02 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:85d026352226e82d36ea400d8e5266afd1dbc0d4de1200d25d3d4012b4e4af41
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:3b1ca9e89f557f32e43e76529de8da986ee003cc0f4a54a7365035a6170e1f94
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:1f3bfd60724100c42a168bed67a8fe8bdc94101d93d0883cded1d3849b1054f6
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:92231b42ede5f888c9c98c7f8ab9c276d59124a2c41030b7b8739f2bf25edec8
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:d5f4690898d9468a22d92f6da530cd28966dffc4e8519de89236954a3815dd02
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:bf8189141c40693c270260e5713202d850ff00db4404912230c4a9201a80aa8c
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:87260cf83b207019a7dbfe2d2f82c5f230a1f156a026a5250a97abfc1de55e00
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:14ace17c2fdc55018dab61c26d1023f8d9794a9b6b9e6d38be339a36dfc732fa
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:7eaa8a0b20cd47c905e3a1444723c0d76c2b156105692af536bfa2e2d1b58b34
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:a25b5384e0d3a6f31ca1047e32332a5b58267cf54a0794b63fb34757e46d2ecb
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:5c9bf563902de42a053c8fc33e9e1f8c0b033fb606ea2f2c0ec012c22f400566
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:dd589aa2abd408d2e9c8f6a0b001db27802f1c3175a95c54f7c2d4993f6ae8d4
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e
```
