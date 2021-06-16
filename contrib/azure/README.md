# Krustlet on Azure

[![Deploy To
Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Falexeldeib%2Fkrustlet%2Face%2Faks%2Fcontrib%2Fazure%2Fazuredeploy.json)



This template deploys and sets up a customized Krustlet instance on an Ubuntu
Virtual Machine. It also deploys a Virtual Network and a Kubernetes cluster
(via AKS).

You can set common Krustlet server properties as parameters at deployment time.

Once the deployment is successful, you can connect to the Kubernetes cluster
using `az aks get-credentials`.

## Prerequisites

You will need to generate an SSH key. This will be used to SSH into the
machines for debugging purposes... Or if you're just curious and want to see
[how the sausage is made](https://en.wiktionary.org/wiki/how_the_sausage_gets_made).

Copy the content of your public key and paste it into the "SSH Public Key"
parameter.
