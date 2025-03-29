## 10 - Explicar el servicio de DHCP  

El servicio de **DHCP** (*Dynamic Host Configuration Protocol*) es un protocolo de red que asigna automáticamente direcciones IP y otros parámetros de configuración a dispositivos en una red.  

### 🔹 ¿Para qué sirve?  
En lugar de asignar manualmente una dirección IP a cada dispositivo, un servidor DHCP lo hace de manera dinámica, evitando conflictos de IP y facilitando la administración de la red.  

### 🔹 ¿Cómo funciona?  
1. **Descubrimiento (Discover):** Un dispositivo nuevo en la red envía una solicitud en busca de un servidor DHCP.  
2. **Oferta (Offer):** El servidor DHCP responde con una dirección IP disponible y otros parámetros (como máscara de subred, puerta de enlace, DNS, etc.).  
3. **Solicitud (Request):** El dispositivo elige la oferta y envía una confirmación al servidor.  
4. **Confirmación (ACK):** El servidor asigna la dirección IP y el dispositivo ya puede comunicarse en la red.  

### 🔹 Beneficios  
✅ **Asignación automática de IPs**  
✅ **Evita conflictos de direcciones**  
✅ **Facilita la gestión de redes grandes**  
✅ **Permite cambiar configuraciones sin afectar a los dispositivos**  

Es súper útil en redes empresariales, hogares con múltiples dispositivos y en cualquier entorno donde no se quiera asignar IPs manualmente.