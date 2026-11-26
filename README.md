<p align="center">
  <a href="https://ag.tavardt.com/mx/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Detector de Enlaces Rotos y Errores de Servidor

[![Detector Enlaces Rotos](https://img.shields.io/badge/TAVARDT-Broken%20Links-5b3cf5.svg)](https://tools.tavardt.com/mx/detector-enlaces-rotos/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Auditoria de hipervinculos internos y salientes, deteccion de errores HTTP 404, enlaces caidos y fugas de presupuesto de rastreo.

***

## Vectores de Riesgo e Impacto Operativo en Enlaces Web

Los hipervinculos rotos con errores HTTP 404 y 500 perjudican la experiencia de usuario y consumen inutilmente el presupuesto de rastreo en Mexico. Los robots de los buscadores abandonan la indexacion al toparse con paginas inexistentes, reduciendo el alcance organico.

Los enlaces salientes que no responden danan la credibilidad del dominio y reducen la puntuacion en motores de respuesta basados en IA. La verificacion tecnica continua protege el flujo interno de autoridad y asegura una navegabilidad optima.

***

## Capacidades Centrales de Auditoria Tecnica

* **Extraccion y Filtrado de Enlaces**: Rastrea las etiquetas href ignorando enlaces locales, llamadas telefonicas y protocolos de correo.
* **Clasificacion de Rutas Internas y Externas**: Separa de forma automatica las URLs del dominio respecto a los hipervinculos que apuntan a terceros.
* **Comprobacion Liviana mediante Metodo HEAD**: Consulta el estado de cada URL sin descargar el contenido para ahorrar ancho de banda.
* **Reintento Inteligente con GET**: Si el servidor remoto bloquea la peticion HEAD con codigos 403 o 405, el auditor repite la prueba con GET.
* **Deteccion Exhaustiva de Errores HTTP**: Registra respuestas 4xx, 5xx y errores de resolucion DNS mostrando un informe diagnostico detallado.
* **Indice de Calidad de Enlaces**: Calcula una puntuacion tecnica de 0 a 100 categorizada en SATISFACTORY, ADVISORY o UNSATISFACTORY.
* **Generacion de Salida Estructurada JSON**: Ofrece soporte para exportar los datos tecnicos a formatos estandarizados de integracion continua.

***

## Instalacion y Ejecucion

Requiere Python 3.8 o superior utilizando unicamente bibliotecas estandar.

```bash
git clone https://github.com/TAVARDT-Mexico/broken-links-checker-mx.git
cd broken-links-checker-mx
python broken_links_scanner.py https://empresa.mx
```

Para generar la salida en formato estructurado JSON en procesos automatizados de auditoria:

```bash
python broken_links_scanner.py https://empresa.mx -j
```

***

## Preguntas Frecuentes (FAQ Tecnico)

### 1. Como perjudican los errores HTTP 404 y enlaces caidos al presupuesto de rastreo?
Los motores de busqueda asignan una cantidad limitada de solicitudes a cada sitio web durante su exploracion. Encontrar enlaces rotos agota este margen en URLs que no existen, retrasando la indexacion de los nuevos contenidos publicados.

### 2. Por que la herramienta efectua consultas HTTP HEAD con alternativa en GET?
El analizador emplea solicitudes HEAD para leer el codigo de estado sin descargar datos innecesarios. Si el servidor remoto rechaza el metodo HEAD con errores 403 o 405, la herramienta ejecuta un reintento mediante GET para evitar falsos positivos.

### 3. De que manera los enlaces internos rotos bloquean la transmision de PageRank?
Los enlaces internos son los canales principales para distribuir autoridad y contexto entre las distintas secciones de una web. Cuando un enlace se rompe, el flujo de valor se interrumpe y las paginas enlazadas pierden visibilidad en las busquedas organicas.

### 4. Que riesgos operativos presenta mantener referencias salientes rotas en el contenido?
Apuntar hacia sitios web dados de baja o comprometidos deteriora la confianza de los usuarios y perjudica la imagen corporativa. Los sistemas modernos de inteligencia artificial valoran la vigencia de las fuentes citadas, penalizando recursos con enlaces rotos.

### 5. Por que es fundamental verificar los enlaces inmediatamente despues de una migracion?
Las modificaciones estructurales y cambios de ruta provocan enlaces desalineados si no se aplican redirecciones adecuadas. El rastreo tecnico detecta de inmediato cualquier codigo 4xx o 5xx, evitando caidas de trafico antes de que afecten al posicionamiento.

***

## Asesoria en Arquitectura de Enlaces y Eficiencia de Rastreo

Para portales de alto volumen y cumplimiento riguroso de los estandares de calidad web W3C, consulte al equipo de **TAVARDT**.

***

## Enlaces Utiles

* **Portal Corporativo:** https://ag.tavardt.com/mx/
* **Suite de Diagnosticos:** https://tools.tavardt.com/mx/
* **Contacto Tecnico:** https://ag.tavardt.com/mx/contacto/

***

### Licencia
Distribuido bajo la Licencia MIT. Consulte el archivo LICENSE para mas detalles.

***

© 2026 TAVARDT. Todos los derechos reservados.
