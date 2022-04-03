------------------
Modo exec usuario
------------------

Switch>
Router>

-----------------------
Modo exec Privilegiado
-----------------------

Switch#
Router#

-----------------------------
Modo de CONFIGURACIÓN GLOBAL
-----------------------------

switch(config)#

--------------------------------
Modo de configuración de líneas
--------------------------------

Switch(config-line)#

-----------------------------------
Modo de configuración de interface
-----------------------------------

Switch(config-if)#


Prácticas y ejemplos:
------------------

Switch>enable -> Permite entrar al modo exec privilegiado.

Switch>dinable -> Sale del modo exec privilegiado.

Switch# configure terminal -> permite entrar al módulo de configuración global:

Enter configuration commands, one per line.  End with CNTL/Z.

Switch(config)# interface vlan 1 -> Entra en el modo de configuración de interface.

Switch(config-if)#line console 0 -> line console 0 -> Permite entrar en el modo de configuración de línea del puerto de la console.

Switch(config-line)# exit

Switch(config) -> sube un nivel, sale del modo configuración de linea al modo de configuración global

Switch(config-line) end -> sube dos niveles, desde el modo de configuración de linea al modo exec privilegiado, también se hace por ctrl + z

Switch(config-line)#interface FastEthernet 0/1 -> se puede trasladar desde el modo de configuración de linea al modo de configuración de interface

Switch(config)#int f 0/1 -> mismo efecto que el comando anterior pero abreviado.

-----------------------
Teclas de acceso rápido:
-----------------------
Pulsación de teclas	Descripción
--
Tabulación      Completa una entrada de nombre de comando parcial.

Retroceso       Borra el carácter a la izquierda del cursor.

Ctrl+D	        Borra el caracter donde está el cursor.

Ctrl+K	        Borra todos los caracteres desde el cursor hasta el final de la línea de comandos.

Esc D	        Borra todos los caracteres desde el cursor hasta el final de la palabra.

Ctrl+U o Ctrl+X	Borra todos los caracteres desde el cursor hasta el comienzo de la línea de comando

Ctrl+W	        Borra la palabra a la izquierda del cursor.
 
Ctrl+A	        Desplaza el cursor hacia el principio de la línea.

Flecha izquierda o Ctrl+B	Desplaza el cursor un carácter hacia la izquierda.

Esc B	        Desplaza el cursor una palabra hacia la izquierda.

Esc F	        Desplaza el cursor una palabra hacia la derecha.

Flecha derecha o Ctrl+F	Desplaza el cursor un carácter hacia la derecha.

Ctrl+E	        Desplaza el cursor hasta el final de la línea de comandos.

Flecha arriba o Ctrl+P	    Recupera los comandos en el búfer de historial, comenzando con la mayoría comandos recientes

Ctrl+R o Ctrl+I o Ctrl+L	Vuelve a mostrar el indicador del sistema y la línea de comando después de que se muestra un mensaje de consola recibido.

-------------------------------------
Tecla ctrl+shift+6 / Ctrl + alt + 6
-------------------------------------

Detendrá la ejecución de un comando después de que el comando ya se haya introducido y el comando se cancela.

----------------
Tecla ctrl + R
----------------

En momentos que se configura un dispositivo, puede darse el caso que alguna veces se muestran logs en la pantalla para quitarlos y volver al prompt, donde estamos solo debemos colocar ctrl + r

















