# Pregunta 21: Tipos de enlace

## **a. Explicación de los enlaces mencionados:**  
- **MPLS** (*Multiprotocol Label Switching*):  
  - Técnica de transporte de datos que utiliza etiquetas para dirigir paquetes eficientemente en redes privadas o de proveedores. Ofrece baja latencia y es ideal para VoIP y VPNs.  
- **LAN to LAN**:  
  - Conexión directa entre dos redes locales, generalmente mediante VPN o enlaces dedicados (ej: fibra óptica).  
- **Microondas**:  
  - Enlace inalámbrico de alta frecuencia (GHz) para distancias cortas/medias (ej: entre edificios). Requiere línea de vista.  
- **VSAT** (*Very Small Aperture Terminal*):  
  - Comunicación satelital para zonas remotas. Alta latencia pero amplia cobertura.  

## **b. Dos tipos de enlace adicionales:**  
1. **Fibra óptica**: Alto ancho de banda, baja latencia, ideal para largas distancias.  
2. **PLC** (*Power Line Communication*): Usa cables eléctricos para transmitir datos (ej: redes domésticas).  

## **c. Ranking de enlaces (1 = mejor, 6 = peor):**  

| Criterio               | MPLS | LAN to LAN | Microondas | VSAT | Fibra óptica | PLC |
|------------------------|------|------------|------------|------|--------------|-----|
| Económico              | 3    | 2          | 4          | 6    | 5            | 1   |
| Performance            | 2    | 3          | 4          | 6    | 1            | 5   |
| Mayor capacidad        | 2    | 3          | 4          | 6    | 1            | 5   |
| Restricciones/config   | 1    | 2          | 4          | 6    | 3            | 5   |
| Soporte a distancia    | 4    | 5          | 3          | 1    | 2            | 6   |
| Menor esfuerzo de config | 4  | 3          | 5          | 6    | 2            | 1   |

## **d. Elección de enlace para escenarios:**  
1. **Call centers con data center central**: **MPLS** (por performance y seguridad).  
2. **Pozos petroleros (15 min/día)**: **VSAT** (por cobertura en zonas remotas).  
3. **Edificios enfrentados**: **Microondas** (línea de vista y bajo costo).  