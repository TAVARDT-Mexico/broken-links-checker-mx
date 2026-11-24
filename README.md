# Detector de Enlaces Rotos y Errores de Servidor

[![Detector Enlaces Rotos](https://img.shields.io/badge/TAVARDT-Broken%20Links-5b3cf5.svg)](https://tools.tavardt.com/mx/detector-enlaces-rotos/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Rastreo de hipervinculos internos y salientes para garantizar navegabilidad y retencion de trafico organico.

Desarrollado y operado por la division de infraestructura de **TAVARDT Mexico**.

***

## Capacidades del Detector de Enlaces Rotos

* **Auditoria de Hipervinculos en Plataformas Web**: Revision rigurosa de catalogo de enlaces internos y externos.
* **Mapeo de Fallas 404 Not Found**: Identificacion inmediata de enlaces rotos que causan rebote de usuarios.
* **Proteccion de Navegabilidad y Conversiones**: Deteccion de enlaces de checkout y navegacion defectuosos en tiendas online.
* **Inventario Detallado de Respuestas**: Clasificacion de codigos HTTP 200, 301, 404 y 500.
* **Puntaje de Salud de Enlaces**: Calificacion de 0 a 100 con listado ordenado de URLs a corregir.

***

## Instalacion y Uso

Requiere Python 3.8 o superior sin librerias de terceros.

```bash
git clone https://github.com/TAVARDT-Mexico/broken-links-checker-mx.git
cd broken-links-checker-mx
python broken_links_scanner.py https://empresa.mx
```

Reporte estructurado en JSON:

```bash
python broken_links_scanner.py https://empresa.mx -json
```

***

## Herramienta en Linea

Para pruebas masivas en servidores en la nube:

* **Detector de Enlaces Rotos en Mexico**
* **[Portal TAVARDT Mexico](https://ag.tavardt.com/mx/)**

***

## Soporte y Consultoria

Para optimizacion tecnica de plataformas segun Estandares Digitales Nacionales y Google Search Central, contacte a **TAVARDT Mexico**.

***

© 2026 TAVARDT. Todos los derechos reservados.
