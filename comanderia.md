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













