# Quickstart
## MCO Updates

Ensure your machines are correctly configured. 

Apply the following MachineConfigOperator (MCO) Settings

```bash
# label master/workers for config-pid
oc label machineconfigpool worker pid-crio=config-pid
oc label machineconfigpool master pid-crio=config-pid

# From the top level directory, run the following command to apply the machine config operator settings
oc kustomize machineconfig | oc apply -f -
```

Watch `oc get MachineConfigPool` to see the progress of the update.

For more information, [Red Hat OpenShift Container Platform Configuration](https://www.ibm.com/docs/en/scalecontainernative?topic=i-red-hat-openshift-container-platform-configuration).
