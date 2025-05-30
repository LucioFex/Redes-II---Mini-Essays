### Cálculo de la direcciones de Red, Host y Broadcast
- [[Dirección de red]]
- [[Dirección de host]]
- [[Dirección de broadcast]]

Este proceso de cálculo requiere que el usuario considere estas direcciones como binarias

![[Pasted image 20250529201327.png]]

Esta diapositiva explica cómo calcular manualmente las direcciones clave dentro de una red IPv4: la dirección de **red**, la **primera y última dirección de host válida**, y la **dirección de broadcast**, utilizando una máscara **/25** (es decir, 25 bits para la red y 7 para hosts).

---
### 🔸 Paso 1: Dirección de red
**IP Base:** `172.16.20.0/25`  
**En binario:**  
`10101100.00010000.00010100.00000000`  
La parte de red son los primeros 25 bits. Todos los bits de host se ponen en 0.  
✅ **Resultado:** `172.16.20.0`
### 🔸 Paso 2: Primera dirección de host válida
Se suma 1 al último bit (al campo de host):  
`10101100.00010000.00010100.00000001`  
✅ **Resultado:** `172.16.20.1`
### 🔸 Paso 3: Dirección de broadcast
Se ponen todos los bits de host en 1 (7 bits → 127):  
`10101100.00010000.00010100.01111111`  
✅ **Resultado:** `172.16.20.127`
### 🔸 Paso 4: Última dirección de host válida
Se resta 1 a la dirección de broadcast:  
`10101100.00010000.00010100.01111110`  
✅ **Resultado:** `172.16.20.126`
### 📌 Conclusión:
Para la red `172.16.20.0/25`:
- 🟦 Dirección de red: `172.16.20.0`
- ✅ Rango de hosts válidos: `172.16.20.1` a `172.16.20.126`
- 🔴 Dirección de broadcast: `172.16.20.127`

Esto sirve para saber cómo se dividen las direcciones en una red y cómo asignarlas correctamente.

