# Pregunta 21: Tipos de enlace

## **a. Explicación de los enlaces mencionados:**  
- **MPLS** (*Multiprotocol Label Switching*):  
  - Técnica de transporte de datos que utiliza etiquetas para dirigir paquetes eficientemente en redes privadas o de proveedores. La red MPLS está ideada para agrupar diferentes tipos de datos trasmitidos mediante la misma red y para mandar paquetes de información que de forma rápida.  Ofrece baja latencia y es ideal para VoIP y VPNs.
  
- **LAN to LAN**:  
  - Conexión directa entre dos redes locales, generalmente mediante VPN, MPLS o enlaces dedicados (ej: fibra óptica).  
  
- **Microondas**:  
  - Enlace inalámbrico de alta frecuencia (GHz) para distancias cortas/medias. Un enlace de microondas es un sistema de comunicación inalámbrico que utiliza ondas electromagnéticas en el rango de microondas para transmitir datos, voz o video entre dos puntos, generalmente a través de un enlace de línea de visión. Operan en la banda de microondas, que típicamente se encuentra entre 1 GHz y 300 GHz. El tipo de enlace puede ser punto a punto (entre dos ubicaciones específicas) o punto multipunto (para conectar múltiples ubicaciones a un punto central).Pueden funcionar en modo simplex (un solo sentido de comunicación), half-duplex (dos sentidos alternos) o full-duplex (dos sentidos simultáneos*). 
  
- **VSAT** (*Very Small Aperture Terminal*):  
  - Los enlaces VSAT, o Terminal de Apertura Muy Pequeña, son enlaces de comunicación satelital que utilizan una antena satelital pequeña para transmitir y recibir datos, voz y video. Generalmente, la red VSAT utiliza una topología en estrella, también llamada arquitectura punto a multipunto, donde una estación de enlace central se comunica con múltiples estaciones remotas a través de satélites.

## **b. Dos tipos de enlace adicionales:**  
1. **Fibra óptica**: Alto ancho de banda, baja latencia, ideal para largas distancias. Estos enlaces se clasifican principalmente en enlaces monomodo (Permite que un solo modo de luz se propague, lo que resulta en menor atenuación y mayor distancia de transmisión. Es ideal para largas distancias y alta velocidad de datos) y multimodo (Permite que múltiples modos de luz se propaguen, lo que puede causar mayor atenuación y limita la distancia de transmisión. Es más adecuado para distancias cortas y velocidades de datos más bajas).
2. **5G**: La tecnología 5G se divide en tres tipos principales de enlaces según la banda de frecuencia utilizada: banda baja (operan en frecuencias más bajas, entre 600 y 900 MHz. Estas bandas ofrecen un alcance más amplio y son ideales para proporcionar cobertura en áreas grandes y densas) , media (utilizan frecuencias entre 1 y 6 GHz. Esta banda ofrece un equilibrio entre alcance y velocidad, siendo adecuada para diversas aplicaciones, como la banda ancha móvil mejorada, las comunicaciones críticas y el IoT masivo) y alta (opera en frecuencias muy altas, entre 24 y 47 GHz. Esta banda permite velocidades de datos extremadamente altas y baja latencia, pero tiene un alcance más limitado. Es ideal para aplicaciones que requieren conexiones de alta velocidad en áreas con alta densidad de usuarios, como eventos deportivos o áreas urbanas). Cada banda ofrece diferentes características y capacidades, lo que permite que la tecnología 5G se adapte a diversos entornos y aplicaciones. 

## **c. Ranking de enlaces (1 = mejor, 6 = peor):**  

| Criterio               | Fibra óptica | MPLS | 5G público | LAN to LAN | Microondas | VSAT |
|------------------------|--------------|------|------------|------------|------------|------|
| **Económico**          | 5            | 4    | 2          | 3          | 1          | 6    |
| **Performance**        | 1            | 2    | 3          | 4          | 5          | 6    |
| **Capacidad**          | 1            | 3    | 2          | 4          | 5          | 6    |
| **Config. restricciones** | 3         | 1    | 4          | 2          | 6          | 5    |
| **Distancia**          | 2            | 4    | 6          | 5          | 3          | 1    |
| **Facilidad config.**  | 6            | 3    | 1          | 2          | 4          | 5    |

---

## **d. Elección de enlace para escenarios:**  
1. **Call centers con data center central**: **MPLS** (por performance y seguridad).  
2. **Pozos petroleros (15 min/día)**: **VSAT** (por cobertura en zonas remotas).  
3. **Edificios enfrentados**: **Microondas** (línea de vista y bajo costo).  