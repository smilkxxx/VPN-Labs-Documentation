# Implementación de Tecnologías VPN utilizando Cisco CSR1000v y FortiGate

## Práctica Final

**Instituto Tecnológico de las Américas (ITLA)**

**Carrera:** Tecnólogo en Ciberseguridad

**Estudiante:** Alvaro Baez Tavera

**Matrícula:** 20211150

**Año:** 2026

---

# Índice

1. Introducción
2. Objetivos
3. Herramientas utilizadas
4. Laboratorios desarrollados
5. Resultados obtenidos
6. Conclusiones
7. Repositorios de GitHub
8. Videos demostrativos
9. Referencias

---

# Introducción

Las Redes Privadas Virtuales (VPN) constituyen una de las tecnologías más importantes para proteger la comunicación entre sedes remotas y usuarios que requieren acceso seguro a los recursos de una organización. Mediante protocolos de autenticación, cifrado y encapsulamiento, las VPN permiten garantizar la confidencialidad, integridad y autenticidad de la información que viaja a través de redes públicas.

Durante el desarrollo de este proyecto se implementaron diferentes tecnologías VPN utilizando routers Cisco CSR1000v con Cisco IOS XE 16.7.1 y dispositivos FortiGate, simulados en GNS3. Cada laboratorio permitió comprender el funcionamiento de protocolos como IPSec, IKEv1, IKEv2, GRE, DMVPN y L2TP, aplicando configuraciones prácticas y verificando la conectividad entre redes remotas.

---

# Objetivos

## Objetivo General

Implementar y validar diferentes tecnologías VPN utilizando Cisco CSR1000v y FortiGate para establecer comunicaciones seguras entre redes remotas.

## Objetivos Específicos

- Implementar VPN Site-to-Site basada en políticas utilizando IPSec.
- Implementar VPN Site-to-Site basada en enrutamiento.
- Configurar túneles GRE protegidos mediante IPSec.
- Implementar DMVPN Fase 2.
- Implementar DMVPN Fase 3.
- Configurar una VPN Client-to-Site mediante L2TP/IPSec.
- Configurar una VPN Site-to-Site utilizando FortiGate.
- Validar el funcionamiento de cada laboratorio mediante pruebas de conectividad.

---

# Herramientas utilizadas

## Software

- Cisco CSR1000v IOS XE 16.7.1
- FortiGate VM
- GNS3
- VPCS
- Kali Linux

## Protocolos

- IPSec
- IKEv1
- IKEv2
- GRE
- DMVPN
- NHRP
- L2TP
- ESP
- AH
- SHA-256
- AES-256

---

# Laboratorios desarrollados

## 1. VPN Site-to-Site Basada en Políticas (Policy-Based VPN)

Se implementó una VPN Site-to-Site basada en políticas utilizando IPSec con IKEv2. La comunicación entre ambas redes se protegió mediante asociaciones de seguridad establecidas a través de IKEv2 y reglas de tráfico definidas mediante políticas.

---

## 2. VPN Site-to-Site Basada en Enrutamiento (Route-Based VPN)

Se implementó una VPN Site-to-Site basada en enrutamiento utilizando una Virtual Tunnel Interface (VTI) protegida mediante IPSec con IKEv1, permitiendo el enrutamiento del tráfico entre ambas sedes utilizando la interfaz del túnel.

---

## 3. VPN Site-to-Site con Túnel GRE sobre IPSec

Se configuró un túnel GRE protegido mediante IPSec utilizando IKEv2. Esta implementación permitió encapsular el tráfico utilizando GRE y posteriormente protegerlo mediante IPSec antes de atravesar la red pública.

---

## 4. DMVPN Fase 2

Se implementó una infraestructura Dynamic Multipoint VPN (DMVPN) Fase 2 utilizando un Hub central y dos Spokes. La comunicación fue protegida mediante IPSec con IKEv1, permitiendo el establecimiento dinámico de túneles entre los dispositivos.

---

## 5. DMVPN Fase 3

Se implementó DMVPN Fase 3 utilizando IPSec con IKEv2. Esta versión incorpora optimizaciones mediante NHRP Redirect y NHRP Shortcut, permitiendo la comunicación directa entre los Spokes sin necesidad de atravesar permanentemente el Hub.

---

## 6. VPN Client-to-Site utilizando L2TP/IPSec

Se implementó una VPN Client-to-Site utilizando L2TP sobre IPSec con IKEv1, permitiendo el acceso remoto seguro desde un cliente hacia la red privada de la organización.

---

## 7. VPN Site-to-Site utilizando FortiGate

Se configuró una VPN Site-to-Site IPSec entre dos dispositivos FortiGate utilizando el asistente IPSec Wizard. Posteriormente se verificó la conectividad entre ambas LAN mediante pruebas de comunicación.

---

# Resultados obtenidos

Durante el desarrollo de las prácticas se logró implementar correctamente diferentes tecnologías VPN sobre Cisco CSR1000v y FortiGate.

Cada laboratorio permitió validar el funcionamiento de los protocolos de autenticación, cifrado y encapsulamiento mediante pruebas de conectividad entre las redes LAN remotas.

Las implementaciones permitieron reforzar los conocimientos relacionados con IPSec, IKEv1, IKEv2, GRE, DMVPN, L2TP y FortiGate, comprendiendo las diferencias entre las VPN basadas en políticas, las VPN basadas en enrutamiento y los túneles GRE protegidos mediante IPSec.

---

# Conclusiones

La implementación de las diferentes tecnologías VPN permitió comprender la importancia de proteger las comunicaciones entre redes remotas mediante protocolos de autenticación y cifrado.

Las prácticas desarrolladas fortalecieron los conocimientos adquiridos sobre IPSec, IKEv1, IKEv2, GRE, DMVPN, L2TP y FortiGate, proporcionando experiencia práctica en la configuración de túneles seguros utilizando Cisco CSR1000v IOS XE 16.7.1 y FortiGate.

Asimismo, se adquirieron habilidades para configurar, verificar y solucionar problemas relacionados con la implementación de VPN Site-to-Site y Client-to-Site, reforzando la comprensión de los mecanismos utilizados para proteger las comunicaciones sobre redes públicas.

---

# Repositorios de GitHub

Los laboratorios desarrollados durante este proyecto se encuentran disponibles en los siguientes repositorios de GitHub:

| Laboratorio | Repositorio |
|-------------|-------------|
| VPN Site-to-Site Basada en Políticas (IPSec IKEv2) | https://github.com/smilkxxx/vpn-policy-based-ipsec-ikev2 |
| VPN Site-to-Site Basada en Enrutamiento (IPSec IKEv1) | https://github.com/smilkxxx/vpn-route-based-ipsec-ikev1 |
| VPN GRE sobre IPSec (IKEv2) | https://github.com/smilkxxx/vpn-gre-over-ipsec-ikev2 |
| DMVPN Fase 2 (IKEv1) | https://github.com/smilkxxx/DMVPN-Phase2-IKEv1 |
| DMVPN Fase 3 (IKEv2) | https://github.com/smilkxxx/DMVPN-Phase3-IKEv2 |
| VPN Client-to-Site L2TP/IPSec (IKEv1) | https://github.com/smilkxxx/L2TP-IPSec-Client-to-Site-IKEv1 |
| VPN Site-to-Site FortiGate IPSec | https://github.com/smilkxxx/FortiGate-Site-to-Site-IPSec-VPN |

---

# Videos demostrativos

Las demostraciones del funcionamiento de todos los laboratorios se encuentran disponibles en la siguiente lista de reproducción de YouTube:

https://www.youtube.com/watch?v=oVUMzzoMRHQ&list=PLKLgCI9UjLn8&pp=sAgC

---

# Referencias

- Cisco Systems. *Cisco IOS XE Security Configuration Guide*.
- Cisco Systems. *Cisco CSR1000v Configuration Guide*.
- Cisco Systems. *GRE over IPSec Configuration Guide*.
- Cisco Systems. *DMVPN Design Guide*.
- Cisco Systems. *IPSec VPN Configuration Guide*.
- Fortinet. *FortiGate Administration Guide*.
- RFC 2401 – Security Architecture for IP.
- RFC 2784 – Generic Routing Encapsulation (GRE).
- RFC 3931 – Layer Two Tunneling Protocol (L2TP).
- RFC 4301 – Security Architecture for the Internet Protocol.

---

# Observación

Cada uno de los laboratorios desarrollados cuenta con su respectivo repositorio de GitHub donde se incluyen la documentación técnica, los scripts de configuración, las capturas de evidencia y los archivos utilizados durante la implementación.
