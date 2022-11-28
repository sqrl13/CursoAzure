# **Instalando Windows Server 2019 en Oracle VM VirtualBox**

## **Requisitos previos** 
1. Contar con la iso de Windows Server 2019
    (Adjunto el link de descarga aqui)
2. Tener un software de virtualización 
    En este caso usaremos VirtualBox 

*Los primeros pasos sirven para configurar diferentes maquinas virtuales.*

### **1.- Primero crearemos una maquina virtual**
Para ello bastará con darle al boton de nueva de nuestro VirtualBox , agregar el nombre que tendrá, donde se guardará la información y cual será la versión. 

En la siguiente pantalla elegiremos la cantidad de RAM que se reservará para el WIndows Server 2019. En mi caso elegí 8 GB pero todo dependerá de la cantidad que tenga tu equipo. 

En la siguente pantalla se creará un disco duro virtual, el tipo será VDI (VirtualBox Disk Image) y el almacentamiento en la unidad será reservado dinámicamente.

Finalmente tendremos en cuenta la ubicación y el tamaño de este. En mi caso le otorgé 100 GB.

### **2.- Configurar la maquina virtual** 

Clicamos en la maquina virtual que vayamos a configurar, para ello nos valdremos del boton de configuración del menú superior de VirtualBox. 

Tendremos que ir al apartado de almacenamiento, dar click el ícono que dice vacio y dar click al disco junto a la frase << Puerto Sata 1 >> y seleccionaremos la opción de << Seleccionar un archivo de disco>>. Escogemos la ubicación donde se encuentra la ISO y aceptamos 

### **3.- Instalar Windows Server 2019**

Iniciamos la maquina virtual, se iniciará la instalación. 

*Es posible que haya pantallazos azules o que se reinicie la maquina virtual, me pasó un par de veces y a al final pude instalarla sin problemas*

Configuraremos el idioma, el tipo de teclado y el formato de Fecha/Hora e instalamos. Te preguntará el sistema operativo. Yo usaré el **Windows Server 2019 Datacenter Evaluation (Expriencia de...)** de x64 a fecha de 07/09/2019

![](https://github.com/sqrl13/CursoAzure/blob/main/VirtualBox/imagenes/2019/1.JPG)


Después de aceptar los terminos y condiciones, tendremos que escoger el tipo de instalación que queremos. En mi caso optaré por la personalizada ya que instalaremos el Windows Server desde cero. 

Luego seleccionamos el disco duro donde se realizará la instalación 

![](https://github.com/sqrl13/CursoAzure/blob/main/VirtualBox/imagenes/2019/2.JPG)

Posteriormente, se iniciará la instalación de Windows Server 2019, este proceso puede demorar algún tiempo dependiendo de los recursos que se le dio a la máquina virtual

Una vez que concluya las tareas le aparecerá esta pantallla 

![imagen3](https://github.com/sqrl13/CursoAzure/blob/main/VirtualBox/imagenes/2019/3.JPG)

Configuramos el usuario Administrador y finalizamos. 

Para ingresar al servidor te pedirá presionar Ctrl + Alt + Supr para ello ve al menú «Entrada->Teclado» y luego da clic en Insertar Ctrl + Alt + Del

Te mostrará la pantalla para ingresar con la contraseña que configuraste y con eso ya hemos terminado la instalación. 

