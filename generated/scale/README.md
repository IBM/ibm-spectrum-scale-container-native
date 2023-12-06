
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:ffa9c4f7f43d8ac142c271780f005e32d0d40db77044fce6a153ddfe37974d6b |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:e3d2f9fb68b2d7cd1faf84002bb73626da10bed5d81f91945a592d41893e2fda |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:39769327dc2a2f276612d79f4b865681d6dd366b78c0760446e7957def6a64f1 |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:f85a1e4153aa9ef91c895a3e5f73b76903e760a26c75a3ecf077b71e6d381906 |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:f85a1e4153aa9ef91c895a3e5f73b76903e760a26c75a3ecf077b71e6d381906 |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:39f62297f1d79f7e0e7fe83ab934db926db3189d0550bdc0a65f3d853752f135 |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:476239363bf644f141612d7a718848d4a5e1e67d1ef1d1a0228deb1330f25d01 |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:c8c7a06ce1c5fa23c1cbd7a0fd891eacd099bc232aa9985ddb183cfe98d1deaf  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:e0f2a5959057d8d6b16802f9a60bfc51de04167f27d92d85eeeabf7c53c86e4e |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:781f86296525f7519d212f8b1887d1a680157b5ebf55f3a989d76579778abb77 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:c8c7a06ce1c5fa23c1cbd7a0fd891eacd099bc232aa9985ddb183cfe98d1deaf |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:bde39274681ae0f3924c77283c120d158174a404f88e0e5913a18d1e0b269d35 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:781f86296525f7519d212f8b1887d1a680157b5ebf55f3a989d76579778abb77 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:7b6d73301bc8b013208d0085e9d21031bea7e6376d5f2cf9834307e298379564 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:57b4ee494ca48342d1ffaf22a166286202b0406b88316e4dcbe87212df6ca8f0 |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:ffa9c4f7f43d8ac142c271780f005e32d0d40db77044fce6a153ddfe37974d6b
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:39f62297f1d79f7e0e7fe83ab934db926db3189d0550bdc0a65f3d853752f135
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:476239363bf644f141612d7a718848d4a5e1e67d1ef1d1a0228deb1330f25d01
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:f85a1e4153aa9ef91c895a3e5f73b76903e760a26c75a3ecf077b71e6d381906
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:bde39274681ae0f3924c77283c120d158174a404f88e0e5913a18d1e0b269d35
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:781f86296525f7519d212f8b1887d1a680157b5ebf55f3a989d76579778abb77
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:e0f2a5959057d8d6b16802f9a60bfc51de04167f27d92d85eeeabf7c53c86e4e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:7b6d73301bc8b013208d0085e9d21031bea7e6376d5f2cf9834307e298379564
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:39769327dc2a2f276612d79f4b865681d6dd366b78c0760446e7957def6a64f1
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:c8c7a06ce1c5fa23c1cbd7a0fd891eacd099bc232aa9985ddb183cfe98d1deaf
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:e3d2f9fb68b2d7cd1faf84002bb73626da10bed5d81f91945a592d41893e2fda
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:57b4ee494ca48342d1ffaf22a166286202b0406b88316e4dcbe87212df6ca8f0
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
```
