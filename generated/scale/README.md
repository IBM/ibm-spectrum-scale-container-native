
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:f520f8e8b265a7cc7ae8d8252336538485d45e84076f0d129c33398f6587af20 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:99ba046ccc9f90777366ebc0dbee55309460d312f68da0f371c176513b5e9592 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:fd1c27c6cf5d34782c5fe718486fab38ba9c8227b4d81961b5e39b692fbd6aa7 |

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:7b9deca9f6313b95f789899d622b967b6d1d9b26d01281cf4528d86535e7153a |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:7b9deca9f6313b95f789899d622b967b6d1d9b26d01281cf4528d86535e7153a |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:3f93641ae75eafdadcc25a476ad635e8a147d9baf61037718ea3bb7439ad4068 |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:f5758e25e6bc4ab45ccb1959bc5b468d25ddce68e70e25e5f6035e7fffbb249e |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-logs@sha256:22c973b4ac5f6ff00a2cadc474c695513ad8246614ab0d145ae5612a6fd769f4  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:3692748b236758ada23f80a67fba5fbbf165acc995ce2da523de51a59a300675 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:7ebe93f44ad6d08a6db9919b775819d2fd2780f3f426ed745736b9247da03ce9 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-logs@sha256:22c973b4ac5f6ff00a2cadc474c695513ad8246614ab0d145ae5612a6fd769f4 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:de8f2f45b5cf33a018e8ffdda25d53f752d0365278587565306eb194696368e5 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:7ebe93f44ad6d08a6db9919b775819d2fd2780f3f426ed745736b9247da03ce9 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:2e04046334baf9be425bb0fa1d04c2d1720d770825eedbdbcdb10d430da4ad8c  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:b4d611100ece2f9bc980d1cb19c2285b8868da261e3b1ee8f45448ab5512ab94 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:bf5a235b67d8aea00f5b8ec24d384a2480e1017d5458d8a63b361e9eeb1608a9 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f25af73ee708ff9c82595ae99493cdef9295bd96953366cddf36305f82555dac |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:a541e6cc2d8b011bb21b1d4ffec6b090e85270cce6276ee302d86153eec0af43 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:db04d298c4171fa3c95a87ff7d474949807205b600530eead06043c49c650e83 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:65a14666cc3dc2ad7516b715f175ddfc18a6f2b5b6c1a3966560b03d6fd02f99 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:f520f8e8b265a7cc7ae8d8252336538485d45e84076f0d129c33398f6587af20
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:3f93641ae75eafdadcc25a476ad635e8a147d9baf61037718ea3bb7439ad4068
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:f5758e25e6bc4ab45ccb1959bc5b468d25ddce68e70e25e5f6035e7fffbb249e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:7b9deca9f6313b95f789899d622b967b6d1d9b26d01281cf4528d86535e7153a
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:65a14666cc3dc2ad7516b715f175ddfc18a6f2b5b6c1a3966560b03d6fd02f99
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:3692748b236758ada23f80a67fba5fbbf165acc995ce2da523de51a59a300675
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-logs@sha256:22c973b4ac5f6ff00a2cadc474c695513ad8246614ab0d145ae5612a6fd769f4
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:7ebe93f44ad6d08a6db9919b775819d2fd2780f3f426ed745736b9247da03ce9
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:de8f2f45b5cf33a018e8ffdda25d53f752d0365278587565306eb194696368e5
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmsensors@sha256:7a9e836c4385ff50c0bae957e1936d2a1a350ffc465bc278371f89f22d9e76b5
cp.icr.io/cp/spectrum/scale/postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:fd1c27c6cf5d34782c5fe718486fab38ba9c8227b4d81961b5e39b692fbd6aa7
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:99ba046ccc9f90777366ebc0dbee55309460d312f68da0f371c176513b5e9592
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:b4d611100ece2f9bc980d1cb19c2285b8868da261e3b1ee8f45448ab5512ab94
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f25af73ee708ff9c82595ae99493cdef9295bd96953366cddf36305f82555dac
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:bf5a235b67d8aea00f5b8ec24d384a2480e1017d5458d8a63b361e9eeb1608a9
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:a541e6cc2d8b011bb21b1d4ffec6b090e85270cce6276ee302d86153eec0af43
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:2e04046334baf9be425bb0fa1d04c2d1720d770825eedbdbcdb10d430da4ad8c
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:db04d298c4171fa3c95a87ff7d474949807205b600530eead06043c49c650e83
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987
```
