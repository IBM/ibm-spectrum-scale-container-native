
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:ebbee83e2c15316c6927ad3654be4ff755bef1cdccb7cc0f55c223e7c433b716
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:2d989634bf3491c81336b2f58c8d27b70eab2a0a5c4ef13048aa83b04afa1728 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:393cab9fa078c272b2b0b5b672d07cbfbf6b0f4609bde7ad823c68601e0478ba |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:393cab9fa078c272b2b0b5b672d07cbfbf6b0f4609bde7ad823c68601e0478ba |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:e7d59b82a30da67a75105048f0c9b0d6fd33f9d2986c7d9a788f340e55e91298 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:eb83a412907a5edd9c68edc9052aabaede79a995df2340214b4a0c2e758de6bd |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:4831c36fe2f9de787930a7c6a412276f35dd55e3e07a0cd36c66be196ed6a11a  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:4159778c647cbb089ee7f03945e442c8740e744c5e7485211122402c4ff4b6ce |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:bab6b3f442736129d96cadece1ecf08ca137449586ee9951d3f34e024becbe18 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:4831c36fe2f9de787930a7c6a412276f35dd55e3e07a0cd36c66be196ed6a11a |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:b0f5896194bd278b9773d533e2f571874f387b42a5fff001f7e9f0a76964398f |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:bab6b3f442736129d96cadece1ecf08ca137449586ee9951d3f34e024becbe18 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:b367ac63080cf5f544ff3410817ac6a594ac1b2a4f7936eb0c140b2a108d2514 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:009d20f17bd99f9ca641b7c60733b842897a6f33854a8e058d229fab610a9a55 |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:1934b811c6048b364859c60a2df5eec5aeef33b85104a5abb4f2251bcc344135 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:ebbee83e2c15316c6927ad3654be4ff755bef1cdccb7cc0f55c223e7c433b716
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:e7d59b82a30da67a75105048f0c9b0d6fd33f9d2986c7d9a788f340e55e91298
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:eb83a412907a5edd9c68edc9052aabaede79a995df2340214b4a0c2e758de6bd
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:393cab9fa078c272b2b0b5b672d07cbfbf6b0f4609bde7ad823c68601e0478ba
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:1934b811c6048b364859c60a2df5eec5aeef33b85104a5abb4f2251bcc344135
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:009d20f17bd99f9ca641b7c60733b842897a6f33854a8e058d229fab610a9a55
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:4159778c647cbb089ee7f03945e442c8740e744c5e7485211122402c4ff4b6ce
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:4831c36fe2f9de787930a7c6a412276f35dd55e3e07a0cd36c66be196ed6a11a
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:bab6b3f442736129d96cadece1ecf08ca137449586ee9951d3f34e024becbe18
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:b0f5896194bd278b9773d533e2f571874f387b42a5fff001f7e9f0a76964398f
cp.icr.io/cp/gpfs/postgres@sha256:0bcc5bbbb2aa9c9b4c6505845918c7eb55d783cf5c1f434fac33012579fb149d
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:2d989634bf3491c81336b2f58c8d27b70eab2a0a5c4ef13048aa83b04afa1728
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:b367ac63080cf5f544ff3410817ac6a594ac1b2a4f7936eb0c140b2a108d2514
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e
```
