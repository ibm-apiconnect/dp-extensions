# DataPower extensions using a manifest for IBM API Connect V10

These Knowledge Center pages describe DataPower extensions:
 - Manifest Main page: https://www.ibm.com/docs/en/api-connect/10.0.1.x?topic=gateway-extensions-manifest
 - How to create a DP extension: https://www.ibm.com/docs/en/api-connect/10.0.1.x?topic=environment-extending-gateway-server-behavior


#Manifest Extension

A  zip file that contain a manifest JSON file and other extension files such as a zip or yaml.  The manifest extension type allows clients to:
 - Deploy 1 or more extensions or policies.
 - Define immediate or deferred deployment for each internal extension entry.
   - Immediate allows users to deploy the extension without having to restart the API Connect Gateway Service.
 - Set global or catalog scope for policies being deployed.
   - When catalog level scope, the user is also requried to push the ref zip file using the toolkit to expose the policy to assembly pallett for that catalog.
 - Deploy the V5E framework for backwards compatibility with V5 artifacts such as user defined policies.
 - Deploy out of the box V5E policies such as invoke 1.5.0 and gatewayscript 1.0.0
