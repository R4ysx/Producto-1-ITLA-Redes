Proyecto de Implementación Empresarial L2/L3
Instituto Tecnológico de las Américas (ITLA) Asignatura: Conmutación y Enrutamiento  Profesor: Onel Luis Pelegrino

Integrantes del Equipo 3
Daniel Dilone - Matrícula: 2024-1648
Raysa Pinales - Matrícula: 2025-0794
Thaziel Brea - Matrícula: 2025-2192
Elianny Adames - Matrícula: 2025-0771

Descripción del Proyecto

Este repositorio contiene los scripts de configuración y la topología implementada en PNETLab correspondientes al Equipo 3 (Red IPv4: 172.20.0.0/15 | IPv6: 2001:25:20::/48). El objetivo principal es desplegar una red confiable, segura y escalable para una mediana empresa.

El proyecto cumple con los siguientes criterios técnicos:

Segmentación: Creación de VLANs por departamentos y distribución mediante VTP (servidor en SWM1 y clientes en la sede central; modo transparente en la sucursal).
Redundancia L2/L3: Implementación de EtherChannel (LACP), STP (RPVST+) y configuración de alta disponibilidad en el gateway utilizando HSRP versión 2, con reparto de carga entre SWM1 y SWM2.
Enrutamiento: Implementación de OSPFv2 (soportando crecimiento multiárea) para la conectividad entre la sucursal y el backbone: área 0 en la sede central y área 1 de tipo stub en la sucursal, con ruta por defecto hacia el ISP.
Seguridad: Restricción de accesos internos y a Internet mediante políticas de seguridad basadas en listas de control de acceso (ACL) estándar y extendidas.
Direccionamiento: Plan de direccionamiento estructurado para IPv4 (VLSM) e IPv6.

Archivos Entregables
Topologia.png: Captura de la topología física en PNETLab.
SWM1.txt: Comandos de configuración del Switch Multicapa 1 (Gateway Principal).
SWM2.txt: Comandos de configuración del Switch Multicapa 2 (Gateway Secundario).
SWAC1.txt: Comandos de configuración del Switch de Acceso 1 (VLAN Docentes).
SWAC2.txt: Comandos de configuración del Switch de Acceso 2 (VLAN Estudiantes).
SWAC3.txt: Comandos de configuración del Switch de Acceso 3 (VLAN Gestión).
SW.txt: Comandos de configuración del Switch del Datacenter.
SWA13.txt: Comandos de configuración del Switch de Acceso de la sucursal (Académicos/Finanzas).
R1-Core.txt: Comandos de configuración del enrutador Core/Backbone.
R2.txt: Comandos de configuración del enrutador de la Sucursal.
ISP.txt: Comandos de simulación del proveedor de Internet.
SERVICIOS.txt: Comandos de configuración del servidor del Datacenter.
Hosts.txt: Comandos de configuración de cada dispositivo host (EST1, DOC1, GES1, FIN1 y ACA1).
Producto 1 Equipo 3: Archivo de topología de PNETLab configurado.
