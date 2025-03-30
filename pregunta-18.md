# 18 - ¿Qué es una DMZ?

Una **DMZ** (Zona Desmilitarizada) en redes informáticas es un área de seguridad intermedia entre la red interna (privada) y la red externa (internet). Su objetivo es agregar una capa extra de protección para los sistemas que deben ser accesibles desde internet, como servidores web, de correo o de bases de datos.

---

## 🔍 ¿Cómo funciona una DMZ?

En una arquitectura de red con DMZ, el firewall separa tres zonas principales:

1 **Red interna (LAN):** La red privada y segura donde están los dispositivos de la empresa.  
2 **DMZ:** Un área intermedia donde se ubican los servidores que necesitan acceso desde internet.

3 **Red externa (WAN/Internet):** La red pública desde donde los usuarios externos acceden a los servicios.

El firewall controla el tráfico entre estas zonas, permitiendo conexiones desde internet solo a la DMZ y restringiendo el acceso directo a la red interna.

🔥 **¿Por qué usar una DMZ?**
✔ **Mayor seguridad:** Si un atacante compromete un servidor en la DMZ, aún no tiene acceso directo a la red interna.  
✔ **Protección de datos sensibles:** La LAN sigue siendo inaccesible para usuarios externos.  
✔ **Mejor control del tráfico:** Se pueden aplicar reglas específicas de acceso y filtrado.

🏢 **Ejemplo de uso de una DMZ**
- Un servidor web colocado en la DMZ permite que los usuarios accedan a un sitio sin exponer toda la red.
- Un servidor de correo en la DMZ recibe correos desde internet sin riesgo directo para la LAN.
- Un servidor proxy en la DMZ filtra el tráfico antes de que llegue a la red interna.

🚨 **Conclusión**  
La DMZ es una estrategia clave en seguridad de redes que minimiza riesgos al exponer servicios al público sin comprometer la red privada. Es como una zona de cuarentena donde los servicios accesibles desde internet están protegidos, pero aislados.
