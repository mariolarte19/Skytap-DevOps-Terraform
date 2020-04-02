# Skytap-DevOps-Terraform💻

## Requerimientos 

* Una maquina virtual ubuntu 
* Terraform v0.12.24
* Terraform-skytap provider v0.14.0

### 1. Instale Terraform en su máquina local

a. Cree una carpeta en su sistema local que se llama terraform y navegue a su carpeta.

`mkdir terraform && cd terraform`

b. [Descargue la ùltima versión de Terraform CLI en su máquina local (en este caso es la 0.12.24)](https://releases.hashicorp.com/terraform/)

El archivo de instalación quedara alojado en la carpeta de descargas que tenga configurada por defecto, por lo que debe entrar a la c arpeta de descargas para extraer el archivo.

`cd $HOME/Downloads`

c. Extraiga el paquete Terraform y copie el archivo binario en su directorio terraform.

`unzip terraform_0.12.24_linux_amd64.zip`<br />
`sudo mv terraform $HOME/terraform`

d. Apunte la variable de entorno $ PATH a su archivo binario Terraform.

`export PATH=$PATH:$HOME/terraform`

e. Verifique que la instalación sea exitosa 

`Terraform --version`

Vera una salida de consola como la siguiente:

`Terraform v0.12.24`

### 2. Descargue el complemento skytap provider 

a. [Descargue la última versión del archivo binario de Skytap Provider.](https://releases.hashicorp.com/terraform-provider-skytap/)

Ingrese a la carpeta de descargas y extraiga el archivo binario del plug-in, para este caso se ha descargado la versión para Linux de 64 bits.

`cd $HOME/Downloads
unzip terraform-provider-skytap_0.14.0_linux_amd64.zip`

b. Cree una carpeta oculta para su complemento.

`mkdir $HOME/.terraform.d/plugins`

c. Mueva el complemento de Skytap Provider a la carpeta oculta que acaba de crear

`mv $HOME/Downloads/terraform-provider-ibm* $HOME/.terraform.d/plugins/`

d. Ingrese a la carpeta occulta y verifique que la instalación se haya terminado

`cd $HOME/.terraform.d/plugins && ./terraform-provider-ibm_*`

Vera una salida como la siguiente:
