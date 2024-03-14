# clearml

## Using CRC to host clearml
- get the ingress cert from crc; replace the value in override.yaml
```
# https://access.redhat.com/documentation/en-us/red_hat_codeready_workspaces/2.1/html/installation_guide/installing-codeready-workspaces-in-tls-mode-with-self-signed-certificates_crw
oc get secret router-ca -n openshift-ingress-operator -o jsonpath="{.data.tls\.crt}" | base64 -d > crc.crt
```
