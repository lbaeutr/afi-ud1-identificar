| | **RFC 3227** | **NIST SP 800-86** | **ENFSI** |
|---|---|---|---|
| **Qué entiende por identificar** | Preguntarse ¿dónde está la evidencia?, listar los sistemas implicados y de cuáles se recogerá, decidir qué es relevante y, ante la duda, recoger más. Seguir preguntándonos qué más puede ser evidencia mientras se trabaja. | Identificar las fuentes potenciales y después adquirirlas; el analista debe saber recorrer una zona física y reconocer fuentes, pensar fuera de ella y tener en cuenta quién es el dueño de cada una. | En la escena, la actividad se divide en identificar, incautar y procesar. |
| **Fuentes que menciona** | Registro y caché, tabla de rutas, ARP, procesos de memoria, ficheros temporales, disco, logs remotos, configuración física y topología de red, medios de archivos. Además de las personas. | Equipos (ordenadores de escritorio y portátiles) y servidores, dispositivos de almacenamiento en red, medios externos de almacenamiento (USB, tarjetas, discos ópticos y discos magnéticos), cámaras y grabadoras. Fuera del equipo: logs de red y de aplicaciones, ISP y copias de seguridad. | Dispositivos en la escena y su red, la memoria volátil de los equipos y sistemas remotos en vivo. |
| **Criterio para decidir qué se protege primero** | El orden de volatilidad, de lo más volátil a lo menos. Recoger primero y analizar después, y no apagar hasta terminar. | Plan que prioriza cada fuente por valor probable, volatilidad y esfuerzo; por lo general, la volatilidad encabeza las prioridades, pero es fundamental considerar aquellos elementos estables que también experimentan cambios, como los logs que se sobrescriben. Esto debe equilibrarse adecuadamente con el impacto real de la organización. | No sigue una regla estricta de orden, sino que prioriza según el riesgo y la situación de cada caso. Busca directamente en las áreas más probables a partir de los argumentos presentados. Se prepara de antemano la captura de lo volátil, porque después de ser incautado puede ser irrecuperable. |




En qué coinciden y en qué se diferencian. Las tres van en la misma línea, hay que documentarlo todo, cuidar la cadena de custodia, no apagar el equipo sin pensar, tener las herramientas preparadas antes de llegar y asegurar primero lo que se pierde antes. La diferencia está en desde dónde se mira cada una.

- La RFC 3227 es la guía del técnico que tiene delante un equipo encendido, dando un orden de volatilidad muy concreto, pero se centra sobre todo en lo que hay dentro del equipo.

- NIST se asoma hacia afuera y recuerda que la evidencia también está en logs, en el ISP o en equipos de terceros, y que el orden de recogida no depende solo de lo volátil que sea un dato, sino también de su valor probable y del esfuerzo que cuesta conseguirlo.

- ENFSI lo plantea como un laboratorio que trabaja con la policía, le preocupa la escena, cómo aislar un dispositivo con radio o wifi sin que se quede sin batería, y prioriza según lo que se investiga.
