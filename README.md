# comandos-elastix
Comandos SSH para elastix importantes


- actualizacion para corregir errores<br>
yum -y update<br>

- abrir el cli<br>
asterisk -rvvvvvv<br>
asterisk -r<br>

- mirar log de que pasa <br>

tail -n 400 /var/log/asterisk/full<br>

- mirar extenciones<br>
 asterisk -rx "sip show peers"<br>

-mirar ip de configuracion<br>
asterisk -rx "sip show peers" |grep 2958548<br>

- mirar data de extenciones<br>
asterisk -rx 'database show' | grep /182<br>

otros<br>
cat /var/log/asterisk/messages | grep -i error | less<br>
iax2 show peers<br>   
iax2 show channels<br>
vim /etc/asterisk/sip.conf<br>
/etc/asterisk/modules.conf<br>
show sip.conf<br>
from-internal-custom<br>
