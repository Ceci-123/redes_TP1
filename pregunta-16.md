# 16 - Explicar el protocolo ARP  

El **Protocolo de Resolución de Direcciones** (ARP - **Address Resolution Protocol**) es un protocolo de red utilizado para encontrar la dirección **MAC** (Media Access Control) de un dispositivo a partir de su dirección **IP** dentro de una red local (LAN).  

---

## 📌 ¿Por qué es necesario ARP?  
Las redes **IP** utilizan direcciones **IP** para identificar dispositivos, pero la comunicación real dentro de una red local se realiza mediante direcciones **MAC**. Como los dispositivos no saben de antemano qué dirección **MAC** corresponde a una **IP** específica, **ARP** se encarga de resolver esta información

## 🔄 Funcionamiento del ARP

1. **Consulta ARP (ARP Request):**  
   Cuando un dispositivo necesita comunicarse con otro en la misma red, envía un mensaje de difusión (broadcast) preguntando:  
   *"¿Quién tiene la IP X.X.X.X? Respóndeme con tu dirección MAC."*

2. **Respuesta ARP (ARP Reply):**  
   El dispositivo que tiene la IP consultada responde directamente al emisor con su dirección MAC.

3. **Almacenamiento en caché:**  
   Para mejorar el rendimiento, las direcciones MAC aprendidas se guardan en una tabla ARP temporalmente, evitando consultas innecesarias.

---

## 🛠 Tipos de ARP

- **ARP estático:** Entradas fijas configuradas manualmente en la tabla ARP.
- **ARP dinámico:** Las direcciones MAC se aprenden automáticamente y se almacenan temporalmente.
- **ARP inverso (RARP):** Permite que un dispositivo descubra su propia IP a partir de su dirección MAC.
- **ARP gratuito (Gratuitous ARP):** Se usa para detectar IP duplicadas o actualizar información en la red.

---

## ⚠ Vulnerabilidades del ARP

ARP no tiene autenticación, lo que lo hace vulnerable a ataques como el **ARP Spoofing**, donde un atacante finge ser otro dispositivo en la red para interceptar tráfico.

---

## 📌 Conclusión

ARP es esencial para la comunicación en redes locales, ya que permite traducir direcciones IP a MAC, facilitando la entrega de paquetes dentro de una LAN. Sin él, los dispositivos no podrían comunicarse eficientemente en redes Ethernet.

