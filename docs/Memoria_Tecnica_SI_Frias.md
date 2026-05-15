# Elaboración de documentación técnica y uso de aplicaciones de propósito general

Ismael Frias Fernandez  
1ºDAW  
Sistemas informáticos  
15/05/2026

# Índice

[**1\. Análisis de necesidades	3**](#análisis-de-necesidades)

1. # Análisis de necesidades {#análisis-de-necesidades}

   Al utilizar Apache Guacamole con Docker resolvemos la necesidad de tener un acceso remoto centralizado, ligero y sobre todo seguro, reduciendo drásticamente el costo de mantenimiento y licencias.  
   

   ## Centralización

   A la empresa le resolvemos la dispersión de accesos. Gracias a Apache Guacamole que nos permite un único punto de entrada seguro a través de nuestro navegador web, pudiendo gestionar tanto los usuarios como permisos y conexiones a múltiples máquinas.   
   

   ## Seguridad y auditoría

   También le resolvemos problemas de seguridad y de auditoría ya que centraliza la autentificación y utiliza HTTPS para asegurar el tráfico web, también podemos registrar y auditar las sesiones de manera remota, o necesitamos abrir el puerto 3389 (RDP) al internet, lo que elimina el vector de ataque más común para ransomware y fuerza bruta.   
   

   ## Ahorro de recursos

   No se requiere instalar software, agentes o VPNs en los dispositivos finales, lo que reduce drásticamente el tiempo de soporte técnico. También al no requerir licencias de acceso de cliente de escritorio remoto para cada máquina, se podrá reducir el costo de licencias Microsoft.  
   Al basarse en HTML 5 garantiza la seguridad al acceder desde cualquier navegador web.  
   El despliegue de Guacamole en contenedores Docker nos permite actualizaciones rápidas, portabilidad y aislamiento, haciendo la infraestructura 100% reproducible y escalable.  
   

   ## ¿Por qué Guacamole \+ Docker y no RDP directo? 

   Porque conectar directamente por RDP a cada máquina es una práctica obsoleta en el entorno actual. Apache Guacamole \+ Docker nos proporciona una mayor ventaja en todos los sentidos.
