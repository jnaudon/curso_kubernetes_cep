# Despliegue de aplicaciones completas

Como hemos estudiado en las unidades anteriores, una aplicación real completa se compone de un conjunto amplio de objetos que definen despliegues, configmaps, servicios, etc. La API de kubernetes no nos ofrece un superobjeto que defina una aplicación completa.

Necesitamos herramientas para gestionar la aplicación completa: empaquetado, instaladores, control de la aplicación en producción, etc. En esta unidad vamos a estudiar [Helm](https://helm.sh/), que es un software que nos permite empaquetar aplicaciones completas y gestionar el ciclo completo de despliegue de dicha aplicación.

Helm usa un formato de empaquetado llamado **charts**. Un chart es una colección de archivos que describen un conjunto de recursos que nos permite desplegar una aplicación en kubernetes.

Los **charts** son distribuidos en distintos repositorios, que podremos dar de alta en nuestra instalación de helm. Para buscar los distintos charts y los repositorios desde los que se distribuyen podemos usar la página [Artifact Hub](https://artifacthub.io/).