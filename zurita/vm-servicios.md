Migración / adecuación / instalación de vm a través de proxmox y crear contenedores internos.

++ Servidor DELL Serv02

----------------
Servidor proxmox
----------------

url: https://192.168.5.21:8006/
user: root
pass:$$developer10


-----------------------
Migración (Portal Web):
-----------------------

Se requiere disgregar el portal web que actualmente se encuentra en un servidor virtualizado con xenserver:

-------------
credenciales:
-------------
ip:192.168.3.110 
user: root
pass: Vp53rv3r2000

user:operador
pass:Vpu53r


1.- Instalar una máquina virtual en el hipervisor (Servidor DELL Serv02) que contenga el portal web:
    
    Docker:
        a) Crear un contenedor (Docker) con el servidor apache y los mods adecuados de manera que gestionen el CMS wordpress, éste contenedor debe resolver peticiones externas provenientes del proxy reverso externo.
        b) Crear un contenedor (Docker) con la base de datos mysql, que sólo escuche peticiones del contenedor al CMS wordpress.

    Seguridad:
        a) gestionar puertos de escucha internos de los contenedores y puertos externos a la vm nativa del hipervisor.
        b) Gestionar fw lógicos con las adecuaciones del caso de manera que se gestionen peticiones únicamente desde un segemento de red lógico creado desde docker.
       
   
        
        
