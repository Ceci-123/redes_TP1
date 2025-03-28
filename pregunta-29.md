# Pregunta 29: Explicar el estándar IEEE 802.3 que regula la red. Cómo se implementa, ventajas y desventajas.

## Introducción
El estándar **IEEE 802.3** establece las especificaciones técnicas para redes Ethernet. Regula:
- Medios físicos (cables)
- Velocidades de transmisión
- Formato de tramas
- Control de acceso al medio (CSMA/CD)

## Implementación

### 1. Componentes de Hardware
| Elemento               | Ejemplos                                      |
|------------------------|-----------------------------------------------|
| Medios de transmisión  | UTP (Cat5e, Cat6), Fibra óptica, Coaxial      |
| Conectores             | RJ-45 (cobre), LC/SC (fibra)                  |
| Transceptores          | NICs, puertos Ethernet en switches/routers    |

### 2. Control de Acceso al Medio (MAC)
- **Trama Ethernet**: Estructura de datos estandarizada
- **Direcciones MAC**: Identificación única de dispositivos
- **Modos de operación**:
  - Half Duplex (CSMA/CD, en desuso)
  - Full Duplex (moderno)

### 3. Dispositivos de Red
- **Switches**:
  - Implementan IEEE 802.3 por puerto
  - Manejo inteligente de tramas
- **Routers**:
  - Interfaces Ethernet para conexión LAN/WAN

### 4. Software
- Drivers de NIC
- Protocolos de red (TCP/IP, ARP, etc.)

## Ventajas
✅ **Estandarización global**  
✅ **Compatibilidad retroactiva**  
✅ **Escalabilidad de velocidades** (10 Mbps → 100 Gbps)  
✅ **Flexibilidad en medios físicos**  

## Desventajas
❌ **CSMA/CD obsoleto** en redes modernas  
❌ **Limitaciones de distancia** en medios de cobre  
❌ **Coste elevado** en implementaciones de alta velocidad