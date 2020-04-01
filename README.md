# Skytap-DevOps-Terraform

## Requerimientos 

* Una maquina virtual ubuntu 
* Terraform v0.12.24
* Terraform-skytap provider v0.14.0

### 1. Instale Terraform en su máquina local

a. Cree una carpeta en su sistema local que se llama terraform y navegue a su carpeta.

`mkdir terraform && cd terraform`

b. Descargue la ùltima versión de Terraform CLI en su máquina local (en este caso es la 0.12.24.

El archivo de instalación quedara alojado en la carpeta de descargas que tenga configurada por defecto, por lo que debe entrar a la c arpeta de descargas para extraer el archivo.

`cd $HOME/Downloads`

c. Extraiga el paquete Terraform y copie el archivo binario en su directorio terraform.

`unzip terraform_0.12.24_linux_amd64.zip`
`sudo mv terraform $HOME/terraform`

d. Apunte la variable de entorno $ PATH a su archivo binario Terraform.

`export PATH=$PATH:$HOME/terraform`

e. Verifique que la instalación sea exitosa

`Terraform --version`

Vera una salida de consola como la siguiente:

`Terraform v0.12.24`
