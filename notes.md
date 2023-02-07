## Notes

#### Installation

```bash
export RG=pixie
export AKSNAME=briar-pixie-aks

az group create -g $RG -l centralus

az aks create --resource-group $RG --name $AKSNAME --node-count 3 --enable-addons monitoring

az aks get-credentials --resource-group $RG --name $AKSNAME

# Copy and run command to install the Pixie CLI.
bash -c "$(curl -fsSL https://withpixie.ai/install.sh)"



```






