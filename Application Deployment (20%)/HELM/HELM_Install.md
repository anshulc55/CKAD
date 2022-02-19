# Helm

## Install helm
curl https://baltocdn.com/helm/signing.asc | sudo apt-key add -
sudo apt-get install apt-transport-https --yes
echo "deb https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
sudo apt-get update
sudo apt-get install helm

##Verify Helm Package
helm version

##Serch for some application like 
helm search <Application Name>

##Install Application via Helm
helm install <Application Name>
- Each installation of a Helm chart to your cluster is referred to as a release.
- With Helm it’s easy to have multiple releases installed to a single cluster, each with its own specific configuration.

helm install <releasename> <ApplicationName>