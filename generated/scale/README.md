
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:fb487a46a6683cc8dc5e33a8104fcf25b1ddded488afb875658050a29a3be91f
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:7265008cabd23c103bdfd1157624ba5ffa6f4ca92d8193a4ef6d30522683fbd2 |


## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:472bed3bddc245ff6409bd6b2dd1f1d9c8a38a1453cf5332834ecb62eff14dec |
| workerX/masterX* | config | cp.icr.io/cp/gpfs | ibm-spectrum-scale-core-init@sha256:472bed3bddc245ff6409bd6b2dd1f1d9c8a38a1453cf5332834ecb62eff14dec |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/gpfs/data-access | ibm-spectrum-scale-daemon@sha256:067ac15ef9279ca33f8cd5133111073c0e2cd60a64214dd9fd8381fd9d4921e5 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/gpfs/data-management | ibm-spectrum-scale-daemon@sha256:1d86645585044e74930b74dd94abd920a73d2e949f312e47601300b166087ac2 |
| workerX/masterX* | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:fa0497f9db5fb7886529f7e843e0769fc911163ef1493fc714dcb18494c65f33  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/gpfs | ibm-spectrum-scale-gui@sha256:51555e3ef9dd730e20b91cb77143d9f1bc72937d374ef716cd020cf0fa0ea067 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:e5b09cb93f7d0a2a4b5dfc6e14820ccf20e321adc1942d44d2fbaf531bba2c32 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/gpfs | postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/gpfs | ibm-spectrum-scale-logs@sha256:fa0497f9db5fb7886529f7e843e0769fc911163ef1493fc714dcb18494c65f33 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/gpfs | ibm-spectrum-scale-pmcollector@sha256:32b665779c5df5c71316884a4cf5f6e5e9c4cfe81afdcb442844c7678cd92327 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/gpfs | ibm-spectrum-scale-monitor@sha256:e5b09cb93f7d0a2a4b5dfc6e14820ccf20e321adc1942d44d2fbaf531bba2c32 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/gpfs/csi | csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/gpfs/csi | csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/gpfs/csi | csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/gpfs/csi | livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/gpfs/csi | csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/gpfs/csi | csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/gpfs/csi | ibm-spectrum-scale-csi-driver@sha256:9c7b9f2c5fc4170eb9e83c888c97f9df441d42145bd6a956b1125391f778f153 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/gpfs | ibm-spectrum-scale-grafana-bridge@sha256:43be2c3f48757c079a991fbd9d5c1365b44ef64303ceee5746b9c854ef026dbd |
| coredns-XXXXX | coredns | cp.icr.io/cp/gpfs | ibm-spectrum-scale-coredns@sha256:c75e1bab2e4f37a14a6cb426bef042c2ad5d7cd09167cfd861810c58e6956d75 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:fb487a46a6683cc8dc5e33a8104fcf25b1ddded488afb875658050a29a3be91f
cp.icr.io/cp/gpfs/data-access/ibm-spectrum-scale-daemon@sha256:067ac15ef9279ca33f8cd5133111073c0e2cd60a64214dd9fd8381fd9d4921e5
cp.icr.io/cp/gpfs/data-management/ibm-spectrum-scale-daemon@sha256:1d86645585044e74930b74dd94abd920a73d2e949f312e47601300b166087ac2
cp.icr.io/cp/gpfs/ibm-spectrum-scale-core-init@sha256:472bed3bddc245ff6409bd6b2dd1f1d9c8a38a1453cf5332834ecb62eff14dec
cp.icr.io/cp/gpfs/ibm-spectrum-scale-coredns@sha256:c75e1bab2e4f37a14a6cb426bef042c2ad5d7cd09167cfd861810c58e6956d75
cp.icr.io/cp/gpfs/ibm-spectrum-scale-grafana-bridge@sha256:43be2c3f48757c079a991fbd9d5c1365b44ef64303ceee5746b9c854ef026dbd
cp.icr.io/cp/gpfs/ibm-spectrum-scale-gui@sha256:51555e3ef9dd730e20b91cb77143d9f1bc72937d374ef716cd020cf0fa0ea067
cp.icr.io/cp/gpfs/ibm-spectrum-scale-logs@sha256:fa0497f9db5fb7886529f7e843e0769fc911163ef1493fc714dcb18494c65f33
cp.icr.io/cp/gpfs/ibm-spectrum-scale-monitor@sha256:e5b09cb93f7d0a2a4b5dfc6e14820ccf20e321adc1942d44d2fbaf531bba2c32
cp.icr.io/cp/gpfs/ibm-spectrum-scale-pmcollector@sha256:32b665779c5df5c71316884a4cf5f6e5e9c4cfe81afdcb442844c7678cd92327
cp.icr.io/cp/gpfs/postgres@sha256:ef257d85f76e48da1c64832459b59fcaba1a4dac97bf5d7450c77753542eee94
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:7265008cabd23c103bdfd1157624ba5ffa6f4ca92d8193a4ef6d30522683fbd2
# IBM Container Storage Interface (CSI) images
cp.icr.io/cp/gpfs/csi/csi-attacher@sha256:5aaefc24f315b182233c8b6146077f8c32e274d864cb03c632206e78bd0302da
cp.icr.io/cp/gpfs/csi/csi-node-driver-registrar@sha256:5244abbe87e01b35adeb8bb13882a74785df0c0619f8325c9e950395c3f72a97
cp.icr.io/cp/gpfs/csi/csi-provisioner@sha256:bb057f866177d5f4139a1527e594499cbe0feeb67b63aaca8679dfdf0a6016f9
cp.icr.io/cp/gpfs/csi/csi-resizer@sha256:5e7cbb63fd497fa913caa21fee1a69f727c220c6fa83c5f8bb0995e2ad73a474
cp.icr.io/cp/gpfs/csi/csi-snapshotter@sha256:bc7be893ecc3ad524194aa6573b2f5c06cd469bdf21a500ab6c99c2ba1c4d64d
cp.icr.io/cp/gpfs/csi/ibm-spectrum-scale-csi-driver@sha256:9c7b9f2c5fc4170eb9e83c888c97f9df441d42145bd6a956b1125391f778f153
cp.icr.io/cp/gpfs/csi/livenessprobe@sha256:88092d100909918ae0a768956cf78c88bc59cd7232720f7cdbdfb5d2e235001e
```
