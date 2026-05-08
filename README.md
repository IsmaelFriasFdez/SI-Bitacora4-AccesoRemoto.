# SI-Bitacora4-AccesoRemoto.
# Bitácora Técnica IV

## Laboratorio de Teletransportación Digital (SSH y RDP)

# Paso 1: Creación archivo .yml

1. Empezaremos creando en nuestro equipo una carpeta de nombre:  *SI\_Bitacora4\_NombreApellido*. (Ejemplo: *SI\_Bitacora4\_IsmaelFrias*).  
      
2. Abrimos nuestra carpeta en VS Code y creamos un archivo .yml con el siguiente nombre \-\> *docker-compose.yml*  
   Este archivo contendrá lo siguiente dentro:

   # \<imagen\>

3. Abre una terminal dentro de la carpeta y ejecuta el comando docker-compose up \-d para que cree todo.  
      
4. Vamos a verificar que todos los contenedores están funcionando correctamente con docker ps

# \<imagen\>
# Paso 2: Ejecución

* Primer paso: Nos conectaremos al contenedor mediante el comando *sh alumno@localhost \-p 2222* o *sh alumno@127.0.0.1 \-p 2222*.  
  La contraseña es : sistemas\_informaticos

  # \<imagen\> 

* Segundo paso: Ahora crearemos una llave de la siguiente manera: *ssh-keygen \-t ed25519 \-C "tu\_correo@ejemplo.com"*

  # \<imagen\>

* Tercer paso: Copiamos la llave pública de la siguiente manera: *ssh-copy-id \-p 2222 alumno@127.0.0.1*

  # \<imagen\>
# Paso 3: Escritorio en el navegador

Existen dos opciones para realizarlo

1. Conexión: Abre tu cliente de Escritorio Remoto (*MSTSC* en Windows o Remmina en Linux) y apunta a localhost:3389.  
     
2. **Web:** Si tu cliente RDP falla, ve a *http://localhost:3000*. Verás el escritorio de Ubuntu dentro de tu navegador gracias a Apache Guacamole.

   # \<imagen\>

3. **Prueba de éxito:** Crea un archivo de texto en el escritorio del contenedor llamado *PRUEBA\_LOGRADA.txt* con un mensaje para el profesor.

   # \<imagen\>
