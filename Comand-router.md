# Comand Router

## ENABLE
Habilitar el router


## CONFIGURE TERMINAL
Entrar a configuracion global 


## HOSTNAME "NAME"
Cambia el nombre del router o switch


## INTERFACE F0/0 
Selecciona el puerto 0 

## DESC LAN " " 
Configura el siguiente comando a la lan marcada 

## Sumarisacion "manualmente"
Sumarisar las redes, de subneteo 

## IP ADD "IP" "MASK"
Agregar al comando anterior (f0/0 o desc lan ) una ip con su mascara 

## NO SHUTDOWN 
Dar de alta el puerto que se tenga seleccionado 

## ip route "ip" "mask" "ruta(serial)/ip"
Decir por que puerto puede enviar la ip que le manden y el sabe que esta por ahi

## no ip route "ip" "mask" "ruta(serial)/ip" 
Dar de baja la ruta del ip 


## do show vlan brie
Ver todas las vlan creadas y que puertos tiene asignados y los entrucamientos

## int range f0/"rango" 1-24
Selecionar un rango de puertos del switch o router

## interface vlan1
selecionar la vlan1 

## ip default-gateway "ip del router"
Dar al switch cual es la ip del router 

## vlan "numero" 
## name "nombre"
Crear una vlan y asignarle un nombre
### nota: El switch solo puede ver el numero de la vlan(etiqueta)

## no vlan "numero"
borrar una vlan 

## switchport mode access
Activar la configuracion de puertos (para configurar vlans, antes debes seleccionar que puertos deseas configurar)

## switchport access vlan "numero"
Le asignas una vlan a los puertos previamente seleccionados

## do show flash
Ver la memoria flash y que archivos tiene (se ve el txt de configuracion y el de las vlan para eliminarlos "si es necesario")


## delete flash:/vlan.dat
Borrar las configuraciones internas de las vlans 
 ### NOTA: la vlan1 puede pasar por cualquier vlan es la predeterminada 
 cuando se borra una vlan se debe pasar todos los puertos de nuevo a la vlan1 sino quedaran deshabilitados 

## Switchport mode trunk
Hacer el modo entrucamiento del switch

## switchport mode trunk allowed vlan  "numero de vlan"
Hacer el modo de entrucamiento del switch solo a las vlan marcadas



