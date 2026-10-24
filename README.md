## RAM535

Ecosistema de ciberseguridad formado por una IA que funciona entera en local y cuatro cuadernos de estudio que se alimentan entre sí. Está orientado a threat hunting, ciberinteligencia, red team y bug bounty, y diseñado con seguridad por defecto.

[Ver el proyecto](https://github.com/Ramiromp95/ram535) · [Ver los cuadernos en línea](https://ramiromp95.github.io/ram535/)

### Componentes

**IA local**
Asistente basado en Gemma y Ollama. Responde con una biblioteca propia y contrasta cada respuesta con fuentes oficiales.

| Biblioteca | Fuentes |
|---|---|
| Ataque y detección | MITRE ATT&CK · Sigma · Atomic Red Team |
| Técnicas con binarios del sistema | LOLBAS · GTFOBins |
| Debilidades y pruebas web | OWASP · CAPEC · CWE |

**Cuadernos de estudio**

| Cuaderno | Contenido |
|---|---|
| Dossier de Amenazas | Glosario vivo de ataques, técnicas y herramientas |
| Cuaderno MITRE | ATT&CK, D3FEND, CAR, ATLAS y AADAPT en español |
| Libro de CVEs | Vulnerabilidades priorizadas con CTEM, CVSS, EPSS y KEV |
| Mapa de estudio | Rutas prácticas de SOC y pentesting |

**Seguridad por diseño**

- Un único módulo puede salir a internet, con lista blanca, solo HTTPS y aprobación del usuario en cada búsqueda
- Defensa contra prompt injection. Todo texto externo se limpia y se trata como datos, nunca como órdenes
- Ventana sin permisos de red, con Content-Security-Policy y motor aislado tras un proxy cerrado
- Registro de cada conexión, panel de seguridad y hallazgos de auditoría documentados

**Tecnologías** · Python · SQLite FTS5 · Ollama · pywebview · MITRE ATT&CK · Sigma · CVSS 3.1 · EPSS · KEV

---

*RAM535 is a security-first cybersecurity ecosystem built around a fully local AI assistant and four interconnected study notebooks for threat hunting, cyber threat intelligence, red team practice and bug bounty learning.*
