
# Instalando packer

Fazer o download do pacote 
``` 
$ wget https://releases.hashicorp.com/packer/1.5.6/packer_1.5.6_linux_amd64.zip
$ unzip packer_1.5.6_linux_amd64.zip && sudo mv packer /usr/local/bin/
```


Agora vamos instalar o plugin VMware vSphere

https://github.com/jetbrains-infra/packer-builder-vsphere/releases

```
$ wget https://github.com/jetbrains-infra/packer-builder-vsphere/releases/download/v2.3/packer-builder-vsphere-iso.linux
$ chmod +x packer-builder-vsphere-iso.linux && sudo mv packer-builder-vsphere-iso.linux /usr/local/bin/
```
Verificando o a versão do packer e validando os arquivos

```
$ packer version
$ packer validate ubuntu-18.04-docker.json
```

Executando

```
packer build ubuntu-18.04-docker.json
```


# Fontes
https://cloud.vmware.com/community/2019/11/12/infrastructure-code-hashicorp-packer-vmware-vmware-cloud-aws/

https://computingforgeeks.com/how-to-install-and-use-packer/

https://www.thehumblelab.com/automating-ubuntu-18-packer/
