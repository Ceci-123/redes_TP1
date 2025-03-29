# 15 - Explicar el protocolo de comunicaciones OSPF  

## 🏛️ Protocolo OSPF (Open Shortest Path First) - RFC 2328  
OSPF (**Open Shortest Path First**) es un protocolo de enrutamiento dinámico que usa el algoritmo de **estado de enlace** (Link-State) para encontrar la mejor ruta en redes grandes. Se basa en el menor **costo** en lugar de la distancia en saltos (hops), lo que lo hace más eficiente que **RIP**.  

---

## 🔹 Características principales de OSPF  
✅ Protocolo de enrutamiento de **estado de enlace**.  
✅ Usa el algoritmo de **Dijkstra** para calcular la mejor ruta.  
✅ Divide la red en **áreas** para mejorar el rendimiento.  
✅ **Convergencia rápida** (se adapta rápidamente a cambios).  
✅ Soporta **VLSM** y **CIDR** (permite sumarización de rutas).

✅ Evita bucles sin necesidad de límite de saltos como RIP.
________________________________________

🔹 **¿Cómo funciona OSPF?**

1️⃣ **Elección del Router Designado (DR) y Backup (BDR)**
   • En redes broadcast, se eligen un DR (Router Designado) y un BDR (Backup) para reducir tráfico.

2️⃣ **Descubrimiento de vecinos**
   • Los routers OSPF intercambian mensajes Hello para descubrir routers vecinos y formar adyacencias.

3️⃣ **Intercambio de bases de datos de estado de enlace (LSDB)**
   • Cada router comparte información de su topología con los demás.

4️⃣ **Cálculo de rutas con el Algoritmo de Dijkstra**
   • Se construye un árbol SPF para encontrar el camino más corto basado en costos de enlace.

5️⃣ **Actualización de rutas solo cuando hay cambios**
   • OSPF no envía actualizaciones periódicas, solo cuando hay cambios en la topología.

________________________________________

🔹 **Áreas en OSPF**
Para mejorar escalabilidad, OSPF divide la red en áreas.

• **Área 0 (Área Backbone):** Centro de la red, todos los demás deben conectarse a ella.
• **Áreas normales:** Conectadas al área 0, reducen el tamaño de las tablas de enrutamiento.
• **Áreas Stub y Totally Stubby:** Reducen la cantidad de rutas intercambiadas.
• **Área NSSA (Not-So-Stubby Area):** Similar a Stub, pero permite rutas externas.

________________________________________

🔹 **Tipos de Mensajes OSPF**
📡 **Hello:** Descubre y mantiene vecinos.  
📡 **DBD (Database Description):** Resume la LSDB.  
📡 **LSR (Link-State Request):** Solicita información de la topología.  
📡 **LSU (Link-State Update):** Envía cambios en la red.  
📡 **LSAck (Link-State Acknowledgment):** Confirma la recepción de actualizaciones.

________________________________________

🔹 **Ejemplo práctico de OSPF**
Imagina una empresa con varias sucursales conectadas.

• Cada router OSPF aprende sobre su entorno y envía información a sus vecinos.  
• El router principal en el centro de la red es el DR.  
• Si una conexión falla, OSPF recalcula rápidamente la mejor ruta alternativa.

________________________________________

🎯 **Resumen**

🔹 Encuentra la mejor ruta basada en costos, no en saltos.  
🔹 Se adapta rápidamente a cambios en la red.  
🔹 Divide la red en áreas para mayor eficiencia.  
🔹 Usa el algoritmo de Dijkstra para el cálculo de rutas.

OSPF es el protocolo ideal para redes empresariales grandes y complejas.
