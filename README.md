# Práctica de App Service para despliegue de una página estática web usando Azure de Microsoft.

![Functions Icon](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/azure-functions-icon.png)

## Breve descripción
Azure Functions es una es un servicio de tipo [PaaS](https://azure.microsoft.com/es-mx/overview/what-is-paas/) y [Serverless](https://azure.microsoft.com/en-us/solutions/serverless/#overview) que se ejecuta en la [nube](https://azure.microsoft.com/es-mx/overview/what-is-the-cloud/) de Azure y ésta  permite hacer microservicios o API's, pero no realiza la funcióin de ***BACKEND***. Se encuentra en el [portal de Azure](https://portal.azure.com/#home). Para más información, se puede consultar la siguiente [página](https://azure.microsoft.com/en-us/services/functions/#features) proporcionada por Azure.


-----------
## Requisitos
 - Tener una cuenta de Azure para realizar la práctica en su [Portal](https://portal.azure.com/#home) (si aún no se cuenta con alguna, se puede hacer el registro en el siguiente [enlace](https://azure.microsoft.com/es-mx/free/)). Esto es ya que el recurso de la Azure Functions está hecha para hacerse como pago por uso por evento (por llamada de este recurso, se cobra). Es decir, se paga por lo que se consume.
 - Contar con una suscripción activa de Azure para poder realizar la práctica. 

----------

## Instrcuciones

1. Entrar a la [página de Azure](https://portal.azure.com/#home) y buscar  la opción **Azure Functions**.

2. En la página de Azure Functions, seleccionar la opción **Crear** y aparecerá un panel de Datos básicos.
![2.1](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/2.1.png)

    - Nos interesa rellenar los paramétros siguiente:

        |Tipo|Realizar|
        |---|---|
        |Grupo de datos|Seleccionar el grupo de recursos al que se le asingnará *Functions*.SI no existe, se puede crear uno. Ejemplo: PrácticaAzureFunctions|
        |Nombre|Introducir el nombre de la función|
        |Publicar|Seleccionar la opción **Código**|
        |Pila de entorno|Es el tipo de lenguaje que ejecutará la aplicación|
        |Región|Seleccionar la región más cercana que esté disponible|
        |Sistema operativo|Seleccionar la opción **Windows** para esta proáctica|
        |Tipo de plan|Consumo (sin servidor)|
    - Esperamos a que cree cuando se activa la opción de "Revisar y crear".
    ![2.2](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/2.2.png)

3. Una vez creada la función, se ingresa al recurso y se busca en el menu lateral la opción **Funciones** para crear una nueva instancia.
    ![3.1](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/3.1.png)
    - Para esta ocasión, se utilizará la plantilla de ***HTTP Trigger***.
    ![3.2](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/3.2.png)
    - Dentro de la plantilla, se debe seleccionar la opción ***Código y prueba*** y se mostrará un código de ejemplo en JavaScript (de acuerdo con las ocpiones que se eligieron durante la creación del servicio).
    ![3.3](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/3.3.png)
    - Para probar la función, se debe ejecutar el código de ejemplo a través del botón ***Probar/ejecutar***. Ahí se realizan las pruebas.
    - Este código puede ser modificado y se debe guardar para que se pueda ejecutar.
    ![3.4](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/3.4.png)
    ![3.5](https://github.com/JohnNadja/Practica-Azure-Functions/blob/main/images/3.5.png)


### Listo, ya está creado el servicio de Azure Functions.

----
# **⚠Importante⚠**: 
### Recordar eliminar el grupo de recursos que se creó en Azure para evitar costos extras no deseados en caso de no ocupar el servicio.
Se puede hacer desde el panel de Azure en inicio y buscando el tipo de recurso que se llama **Grupo de Recursos**.


## Hasta aquí la finalización de la práctica.