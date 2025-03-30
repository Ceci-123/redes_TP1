
## 11 - Explicar el servicio de DNS  

El servicio de **DNS** (*Domain Name System*) es un sistema que traduce nombres de dominio (como `google.com`) en direcciones IP (como `142.250.190.46`), permitiendo que los dispositivos se comuniquen en la red sin necesidad de recordar números complicados.  

### 🔹 ¿Para qué sirve?  
Los dispositivos en Internet se identifican con direcciones IP, pero recordar esas direcciones sería un problema. El DNS hace que podamos usar nombres fáciles de recordar en lugar de IPs.  

### 🔹 ¿Cómo funciona?  
1. **Consulta:** Cuando escribes `google.com` en el navegador, tu dispositivo pregunta al servidor DNS cuál es la IP de ese dominio.  
2. **Búsqueda en caché:** Si la IP ya está guardada en caché, se usa directamente; si no, se consulta a servidores DNS más altos en la jerarquía.  
3. **Respuesta:** El servidor DNS responde con la IP correspondiente.  
4. **Conexión:** Tu dispositivo usa esa IP para conectarse al servidor y cargar la página.  

### 🔹 Tipos de Servidores DNS  
📌 **Recursivo:** Se encarga de buscar la IP consultando otros servidores si no tiene la respuesta.  
📌 **Raíz:** Son la base de la jerarquía DNS y dirigen las consultas a los servidores adecuados.  
📌 **TLD (Top-Level Domain):** Administran dominios de nivel superior, como `.com`, `.org`, `.net`.  
📌 **Autoritativo:** Contienen la información oficial sobre un dominio específico.  

### 🔹 Beneficios  
✅ **Permite usar nombres amigables en vez de IPs**  
✅ **Acelera el acceso a sitios web gracias a la caché**  
✅ **Mejora la seguridad con filtros de phishing o malware**  
✅ **Es clave para el funcionamiento de Internet**  

Sin el DNS, navegar en Internet sería como recordar los números de teléfono de todos tus contactos en vez de usar sus nombres. 
