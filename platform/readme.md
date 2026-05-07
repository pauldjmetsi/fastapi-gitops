# Platform setup

## Prerequisites
For the FastAPI app self-signed certificate to work, you will need to install the **clusterissuer.yaml** file in the platform directory onto your cluster.

**Command to run:**
```
# apply the clusterissuer.yaml file
kubectl apply -f clusterissuer.yaml

# verify the cluster issuer 'selfsigned-cluster-issuer' is installed
kubectl get clusterissuer
```

Next, you will have to install the certificate onto your desktop computer. 

### Install the Root CA Certificate on your local machine (Windows)
1. Double click on the file you just created
2. Click on the Install Certificate button
3. Click on the Local Machine button
4. Select the option to Place all certificates in the following store
5. Browse and select Trusted Root Certification Authorities
6. Click Finish