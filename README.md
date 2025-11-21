# despr2_1_apache
> Repositorio creado para la práctica "Actividad 2.1 - Instalación y despliegue básico en Apache".
## Descripición del proyecto
El objetivo de esta práctica es instalar y configurar Apache en una máquina virtual (Ubuntu 22.04) y desplegar un sitio web estático sencillo con navegación entre páginas, imágenes y estilos.

## Pasos seguidos para la instalación y despliegue
+ 1 Creación de la mv:
    + Crea una VM como clon enlazado de la VM base Ubuntu-Server-Base.ova proporcionada en el repositorio del curso:
    ![clonado de la mv](image.png)
    + Configuración de la red:
    ![borrado de antiguas reglas](image-1.png)
    ![Nuevas reglas con puertos diferentes](image-2.png)
    + Iniciar la mv y acceder al host por SSH
    ![Inicio a la mv](image-4.png)
    ![Acceso por ssh](image-3.png)
+ 2 Preparación del entorno:
    + Actualización de paquetes:
    ![Actualización de paquetes](image-5.png)
    + Instalación apache2: 
    ![instalacion apache](./image-6.png)
    + Configuración del firewall para permitir tráfico HTTP y HTTPS:
    ![Config firewall](image-7.png)
    + Verificacion de las reglas aplicadas:
    ![alt text](image-8.png)
    + Configuración y habilitación del tráfico ssh, HTTP y HTTPS: 
    ![alt text](image-9.png)
    + Habilitación del firewall:
    ![alt text](image-10.png)
3. Comprobación básica:
    + Comprobación que el servicio está activo:
    ![alt text](image-11.png)
    + Visualización de http://localhost:8081/
    ![alt text](image-12.png)

4. Desplegación del sitio de ejemplo: 
    + Copia los archivos del sitio de ejemplo a /var/www/html/:
    ![alt text](image-17.png)
    ![alt text](image-18.png)
    + Comprobación del localhost:8081
    ![alt text](image-19.png)
    ![alt text](image-20.png)
    + Ajustar permisos y propiedades de los archivos: 
    ![alt text](image-21.png)

5. Comprobación final: 
    ![alt text](image-22.png)

6. Creación de snapshot:
    ![alt text](image-23.png)
    ![alt text](image-24.png)

## Problemas encontrados durante la configuración y despligue, y su solución
No he encontrado problemas significativos al realizar las tareas concretas de la práctica. La única dificultad fue que, en el ordenador del instituto, las descargas tardaban tanto que a veces tenía que apagar la máquina virtual y volver a empezar, lo que generaba un ciclo repetitivo de descargas.