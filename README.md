# comandos-elastix
Comandos SSH para elastix importantes


- actualizacion para corregir errores
yum -y update

- abrir el cli
asterisk -rvvvvvv
asterisk -r

- mirar log de que pasa 

tail -n 400 /var/log/asterisk/full

- mirar extenciones
 asterisk -rx "sip show peers"

-mirar ip de configuracion
asterisk -rx "sip show peers" |grep 2958548

- mirar data de extenciones
asterisk -rx 'database show' | grep /182

otros
cat /var/log/asterisk/messages | grep -i error | less
iax2 show peers   
iax2 show channels
vim /etc/asterisk/sip.conf
/etc/asterisk/modules.conf
show sip.conf
from-internal-custom
