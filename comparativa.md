# Comparativa de las normas

| | **RFC 3227** | **NIST SP 800-86** | **ENFSI** |
|---|---|---|---|
| **Qué entiende por identificar** | Preguntarse ¿dónde está la evidencia?, listar los sistemas implicados y de cuáles se recogerá, decidir qué es relevante y, ante la duda, recoger más. Seguir preguntándonos qué más puede ser evidencia mientras se trabaja. | Identificar las fuentes potenciales y después adquirirlas; el analista debe saber recorrer una zona física y reconocer fuentes, pensar fuera de ella y tener en cuenta quién es el dueño de cada una. | Actividad de la escena (identificar, incautar, procesar): asegurar la zona, orientar la búsqueda según lo que se alega y valorar lo hallado. |
| **Fuentes que menciona** | Registro y caché, tabla de rutas, ARP, procesos , memoria, ficheros temporales, disco, logs remotos, configuración física y topología de red, medios de archivos. Además de las personas. | Equipos (ordenadores de escritorio y portátiles) y servidores, dispositivos de almacenamiento en red, medios externos de almacenamiento (USB, tarjetas, discos ópticos y discos magnéticos), cámaras y grabadoras. Fuera del equipo: logs de red y de aplicaciones, ISP y copias de seguridad. | Dispositivos en la escena y su red, la memoria volátil de los equipos y sistemas remotos en vivo. |
| **Criterio para decidir qué se protege primero** | El orden de volatilidad, de lo más volátil a lo menos. Recoger primero y analizar después, y no apagar hasta terminar. | Plan que prioriza cada fuente por valor probable, volatilidad y esfuerzo; por lo general, la volatilidad encabeza las prioridades, pero es fundamental considerar aquellos elementos estables que también experimentan cambios, como los logs que se sobrescriben. Esto debe equilibrarse adecuadamente con el impacto real de la organización. | No sigue una regla estricta de orden, sino que prioriza según el riesgo y la situación de cada caso. Busca directamente en las áreas más probables a partir de los argumentos presentados. Se prepara de antemano la captura de lo volátil, porque después de ser incautado puede ser irrecuperable. |

## En qué coinciden y en qué se diferencian

**Coinciden** en documentar todo, mantener la cadena de custodia, no apagar sin pensar, llevar las herramientas preparadas y asegurar primero lo que antes se pierde.

**Se diferencian** en el punto de vista:

- **RFC 3227:** es la guía de quien tiene delante un equipo encendido; da un orden de volatilidad muy concreto, pero casi todo su detalle está en el propio sistema.
- **NIST SP 800-86:** mira hacia fuera (logs, ISP, copias, terceros) y añade que el orden no depende solo de la volatilidad.
- **ENFSI:** piensa en la escena y en el laboratorio: asegurar la zona, aislar dispositivos con radio y priorizar según el caso.

**Qué se escaparía con una sola norma:** solo con la RFC 3227 me centraría en la RAM y olvidaría que los logs y las copias rotan; solo con NIST me faltaría el orden de volatilidad y el control de la escena; y solo con ENFSI me faltaría el detalle técnico de qué recoger primero.