# SI-Bitacora4-AccesoRemoto.
# Bitácora Técnica IV

## Laboratorio de Teletransportación Digital (SSH y RDP)

# Paso 1: Creación archivo .yml

1. Empezaremos creando en nuestro equipo una carpeta de nombre:  *SI\_Bitacora4\_NombreApellido*. (Ejemplo: *SI\_Bitacora4\_IsmaelFrias*).  
      
2. Abrimos nuestra carpeta en VS Code y creamos un archivo .yml con el siguiente nombre \-\> *docker-compose.yml*  
   Este archivo contendrá lo siguiente dentro:

   <img width="591" height="648" alt="Captura de pantalla 2026-05-08 141600" src="https://github.com/user-attachments/assets/8e512ce2-99b5-45ed-b4da-d13c21c97f8f" />

3. Abre una terminal dentro de la carpeta y ejecuta el comando docker-compose up \-d para que cree todo.  
      
4. Vamos a verificar que todos los contenedores están funcionando correctamente con docker ps
<img width="1533" height="104" alt="Captura de pantalla 2026-05-08 141841" src="https://github.com/user-attachments/assets/84cc47bd-a3d7-4fc7-ba22-772347bb0b27" />

# Paso 2: Ejecución

* Primer paso: Nos conectaremos al contenedor mediante el comando *sh alumno@localhost \-p 2222* o *sh alumno@127.0.0.1 \-p 2222*.  
  La contraseña es : sistemas\_informaticos

  <img width="597" height="152" alt="Captura de pantalla 2026-05-08 142104" src="https://github.com/user-attachments/assets/6b8ca243-1c76-415a-86f5-5bcd2964d671" /> 

* Segundo paso: Ahora crearemos una llave de la siguiente manera: *ssh-keygen \-t ed25519 \-C "tu\_correo@ejemplo.com"*

  <img width="678" height="357" alt="Captura de pantalla 2026-05-08 142643" src="https://github.com/user-attachments/assets/e80aac33-b80b-4504-b12b-61cad0e4eee9" />

* Tercer paso: Copiamos la llave pública de la siguiente manera: *ssh-copy-id \-p 2222 alumno@127.0.0.1*

  <img width="821" height="244" alt="Captura de pantalla 2026-05-08 142712" src="https://github.com/user-attachments/assets/b0b64e0b-0c62-46c5-b63e-e607884e4f2f" />
# Paso 3: Escritorio en el navegador

Existen dos opciones para realizarlo

1. Conexión: Abre tu cliente de Escritorio Remoto (*MSTSC* en Windows o Remmina en Linux) y apunta a localhost:3389.
   <img width="405" height="244" alt="Captura de pantalla 2026-05-08 143525" src="https://github.com/user-attachments/assets/d555946f-d302-4254-a851-27b1fa787e7d" />

     
3. **Web:** Si tu cliente RDP falla, ve a *http://localhost:3000*. Verás el escritorio de Ubuntu dentro de tu navegador gracias a Apache Guacamole.


4. **Prueba de éxito:** Crea un archivo de texto en el escritorio del contenedor llamado *PRUEBA\_LOGRADA.txt* con un mensaje para el profesor.

   <img width="779" height="470" alt="Captura de pantalla 2026-05-08 144048" src="https://github.com/user-attachments/assets/1484ce2d-7ac5-4edb-89ad-160bfefc3ee7" />
