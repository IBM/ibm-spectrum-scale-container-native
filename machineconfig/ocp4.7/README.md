# Quickstart

## Machine Config Operator Updates for OpenShift Container Platform 4.7

The following Machine Configuration files are prerequisite to an IBM Spectrum Scale Container Native installation on Red Hat OpenShift Container Platform 4.7.
For more information, see [Red Hat OpenShift Container Platform Configuration](https://www.ibm.com/docs/en/scalecontainernative?topic=i-red-hat-openshift-container-platform-configuration) on IBM Spectrum Scale Container Native official documentation.

### Create and Apply the MachineConfigOperator (MCO) Settings

From the top level directory, the following command will build a YAML file to apply the machine config operator settings for Red Hat OpenShift Container Platform 4.7. This YAML is supported for x86_64 and ppcle64 architectures.

```bash
oc kustomize ocp4.7 | oc apply -f -
```

For s390x architecture, issue the following command to build a YAML file to apply the machine config operator settings for Red Hat OpenShift Container Platform 4.7.

```bash
oc kustomize ocp4.7/s390x | oc apply -f -
```

### Pre-Generated MachineConfigOperator files for specific architectures (x86_64, ppc64le, s390x)

- If you are running x86_64, apply the following:

  ```bash
  oc apply -f https://raw.githubusercontent.com/IBM/ibm-spectrum-scale-container-native/v5.1.1.1/generated/mco/ocp4.7/mco_x86.yaml
  ```

- If you are running ppc64le, apply the following:

  ```bash
  oc apply -f https://raw.githubusercontent.com/IBM/ibm-spectrum-scale-container-native/v5.1.1.1/generated/mco/ocp4.7/mco_ppc64le.yaml
  ```

- If you are running s390x, apply the following:

  ```bash
  oc apply -f https://raw.githubusercontent.com/IBM/ibm-spectrum-scale-container-native/v5.1.1.1/generated/mco/ocp4.7/mco_s390x.yaml
  ```
  