# Protocolo de configuración dinámica de host.
### Dynamic Host Configuration Protocol
#### ¿Qué es?
Es un protocolo de "*configuración dinámica de host*", es de [[cliente-servidor]].
Este protocolo es el antecesor de [[BOOTP]].
#### ¿Qué hace?
Proporciona automáticamente un host de protocolo de internet ([[IP]]) y otra información de configuración relacionada.

Permite el inicio de sistemas "sin disco". Usa ambientes sin cambios de frecuencia (estáticos).
###### Info. Config. Relacionada:
- Máscara de subred (**[[default subnet mask]]**)
- Puerta de enlace predeterminada (**[[default gateway]]**)
#### ¿Cómo se asignan las direcciones IP?
Dinámicamente, dentro de un pool de direcciones que el "administrador" configura.
La concesión de una dirección IP tiene cierta validez.
- Osea, DHCP hace una asignación de IP temporal.
#### ¿Cuáles son las ventajas?
- Evita que los usuarios tengan que configurar manualmente:
	- Direcciones IP.
	- Sub-máscaras de red.
	- Direcciones de Gateway.
- Reduce el margen de error humano en la configuración.
- Administración centralizada.
	- Control del espacio y uso de direcciones de una red.
	- Contiene configuraciones avanzadas (reservas de direcciones).
### Detalle técnico de DHCP: [[Funcionamiento de DHCP]]

