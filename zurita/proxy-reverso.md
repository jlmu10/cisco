1.- Instalación de proxy reverso:

Maquina para instalar el proxy reverso:

Servidor proxmox:
url: https://192.168.3.14:8006
-----------
observación: Ésta es maquina es una pc, está instalado proxmox para crear maquinas virtuales que va a contener el proxy reverso externo y el proxy reverso interno (separados)
-----------

user:root
pass: $$developer10

-------------------------------
Solicitud proxy reverso externo:
-------------------------------

a) Instalar maquina virtual con la imagen de debian 11 (cargada en el hipervisor):

#1
Servidor: Proxy Reverso Externo
Sistema Operativo: GNU/LINUX Debian versión 11.x 
Hostname: prvp
Usuario: usuprvp
core: 1
Almacenamiento solicitado: 30GB

Tipo de particionamiento LVM

    - /boot    ->500mb
    - /swap    ->2GB
    - /raiz    ->8GB
    - /var     ->8,5GB
    - /var/log ->8GB
    - /tmp     ->3GB

---------------------------
Direcciones ip disponibles:
---------------------------

192.168.3.16 / 192.168.3.17

==============


Una vez instalado el proxy reverso, debe configurarse el certificado de validación de dominio (Letsencrypt), mientras se adquiere el certificado de propiedad organizacional.

El proxy reverso (nginx) debe tramitar las peticiones externas hacia:

++ portal web
++ sigevic

Seguridad:
        a) Se requiere asegurar el proxy reverso con fw lógicos (ufw o fail2ban)
        b) Adecuar los archivos de configuración y el sistema operativo contra ataques ddos, deshabilitar metodos http no deseados, clickjacking, cross site scripting (xss / x-xss) y otros
        c) instalar todas las librerías y mods de aseguramiento del proxy reverso.
        
Incluir reglas de seguridad interna del hipervisor (firewall, redes virtuales)

-------------------------------
Solicitud proxy reverso interno:
-------------------------------

Sin especificar aún.


Incluir reglas de seguridad interna del hipervisor (firewall, redes virtuales)




