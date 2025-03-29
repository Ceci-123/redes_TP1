# 14 - Explicar el protocolo Spanning Tree  

## 🌳 Protocolo Spanning Tree (STP) - IEEE 802.1D  
El **Spanning Tree Protocol (STP)** es un protocolo de red que previene bucles en redes conmutadas (switches) al desactivar enlaces redundantes.  

---

## 🔹 ¿Por qué es necesario?  
En una red con múltiples switches, pueden existir caminos redundantes para mejorar la disponibilidad. Sin STP, estos caminos pueden generar bucles que:  
❌ **Saturan la red** con tráfico duplicado.  
❌ **Causan colisiones** y fallos en la comunicación.  
❌ **Evitan la correcta entrega** de paquetes a los dispositivos.  

📌 **STP desactiva temporalmente los enlaces redundantes hasta que sean necesarios** (por ejemplo, si un enlace principal falla).  

---

## 🔹 ¿Cómo funciona STP?  

1️⃣ **Elección del Root Bridge**  
   - Todos los switches eligen uno como **Root Bridge** (switch principal) basado en la **prioridad más baja** (Bridge ID).  

2️⃣ **Cálculo del camino más corto**  
   - Se elige el camino más eficiente desde cada switch hacia el **Root Bridge**, basado en el **costo del enlace** (menor costo = mejor camino).  

3️⃣ **Desactivación de enlaces redundantes**  
   - STP pone en estado de **Blocking** los enlaces que podrían generar bucles.  

4️⃣ **Monitoreo y reactivación**  
   - Si un enlace principal falla, **STP reactiva un enlace bloqueado** para restaurar la conectividad.  

---

## 🔹 Estados de un puerto en STP  
| Estado    | Función |
|-----------|----------------------------------|
| **Blocking**   | Bloquea tráfico para evitar bucles. |
| **Listening**  | Evalúa si debe activarse o no. |
| **Learning**   | Aprende direcciones MAC antes de reenviar tráfico. |
| **Forwarding** | Reenvía tráfico normalmente. |
| **Disabled**   | Puerto apagado o sin conexión. |

---

## 🔹 Variantes de STP  
🚀 **RSTP (Rapid STP - IEEE 802.1w):** Versión mejorada con convergencia más rápida.  
🚀 **MSTP (Multiple STP - IEEE 802.1s):** Maneja múltiples VLANs eficientemente.  
🚀 **PVST (Per VLAN STP - Cisco):** Ejecuta STP por cada VLAN en switches Cisco.  

---

## 🔹 Ejemplo práctico  
Imagina **tres switches conectados en un triángulo**. Sin STP, los datos podrían circular en un bucle infinito. Con STP:  

✔️ **Un switch es elegido Root Bridge.**  
✔️ **Se selecciona el camino más corto a ese switch.**  
✔️ **Un enlace se bloquea para evitar bucles.**  

📌 **Si un enlace principal falla, STP habilita el enlace bloqueado y mantiene la red operativa.** 💡  

---

## 🎯 Resumen  
🔹 **Evita bucles** en redes conmutadas.  
🔹 **Selecciona un Root Bridge** y bloquea enlaces redundantes.  
🔹 **Reactiva enlaces bloqueados** si hay fallos.  
🔹 **RSTP es una versión más rápida y eficiente.**  

STP es clave en redes con switches para evitar caos y mantener la estabilidad. 🚀  
