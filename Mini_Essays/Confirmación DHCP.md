Para terminar, el servidor confirma los parámetros [[TCP-IP]] y los envía nuevamente al cliente [[DHCP]], esta vez con el paquete **DHCPACK** (DHCP Acknowledged).

Este paquete contiene otros datos:
- Servidores [[DNS]].
- [[SMTP]].
- [[POP3]].

El cliente DHCP guarda localmente los datos recibidos y se conecta a la red.

Otra cosa, si el servidor no cuenta con ninguna dirección para ofrecer, respondería con **DHCPNAK** (DHCP not acknowledged).
