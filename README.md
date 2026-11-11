<img src="images/neteclogo.png" alt="logo" width="300"/>

# Introducción al Ethical Hacking

## Plataforma de laboratorios

Te damos la bienvenida a la **plataforma de laboratorios** del curso **Introducción al Ethical Hacking**. Aquí podrás explorar diferentes tecnologías a través de prácticas guiadas. ¡Desarrolla tus habilidades y lleva tus conocimientos al siguiente nivel!

## Descripción del curso

Taller práctico introductorio enfocado en técnicas de reconocimiento y recopilación de información utilizadas en Ethical Hacking. Mediante Google Dorking, Shodan y Nmap, los participantes aprenderán a localizar información pública, identificar dispositivos y servicios expuestos en Internet y realizar escaneos básicos de red para reconocer posibles riesgos de seguridad.

**Duración:** 2 horas (120 minutos), 100% práctica.

## Objetivos del curso

Aplicar operadores avanzados de búsqueda mediante Google Dorking, utilizar Shodan para identificar dispositivos y servicios expuestos en Internet, ejecutar escaneos básicos de red con Nmap e interpretar la información obtenida para reconocer posibles puntos de exposición y riesgos de seguridad.

## Perfil de audiencia

Estudiantes, profesionales de TI, administradores de sistemas y redes, y personas interesadas en iniciarse en Ethical Hacking, particularmente en técnicas básicas de reconocimiento, recopilación de información y análisis de exposición de sistemas.

## Prerrequisitos

- Conocimientos básicos de redes TCP/IP, direcciones IP, puertos y servicios de red.
- Familiaridad con la navegación web y el uso básico de sistemas operativos.
- Haber culminado el curso Ethical Hacking disponible en Cisco NetAcad.

## Lista de laboratorios

Cada uno de estos laboratorios está diseñado para ofrecerte una experiencia práctica. Haz clic en los enlaces para comenzar.

### [Práctica 1. OSINT | Introducción a Google Dorks para búsqueda avanzada de información](Capitulo01/README.md)

  - **Descripción**: búsquedas con `site:`, `filetype:`, `intitle:` e `inurl:` sobre sitios públicos y un sitio de prueba autorizado, revisión de la Google Hacking Database y propuesta de mitigación.
  - ⏱️ **Duración estimada**: 40 min.

### [Práctica 2. Introducción a búsqueda de dispositivos en Internet con Shodan](Capitulo02/README.md)

  - **Descripción**: búsquedas con filtros de puerto, servicio y país, análisis de la ficha de un host autorizado y relación de servicios expuestos con riesgos.
  - ⏱️ **Duración estimada**: 40 min.

### [Práctica 3. Introducción al escaneo de red con Nmap](Capitulo03/README.md)

  - **Descripción**: descubrimiento de hosts, escaneo de puertos y detección de servicios con comandos de Nmap en una red de laboratorio simulada con Google AI Studio.
  - ⏱️ **Duración estimada**: 40 min.

### Distribución del tiempo

| Práctica | Herramienta | Duración |
|---|---|---|
| 1. OSINT con Google Dorks | Google Search | 40 min |
| 2. Búsqueda de dispositivos con Shodan | Shodan | 40 min |
| 3. Escaneo de red con Nmap | Nmap (simulador en Google AI Studio) | 40 min |
| **Total** | | **120 min** |

## Instrucciones generales del laboratorio

1. Antes del taller, preparar el equipo y las cuentas con la [Guía de configuración](Setup_Guide.md).
2. Cada práctica está en su carpeta `CapituloNN` con su `README.md` y la carpeta `recursos`. Para descargar un archivo, abrirlo y seleccionar **Download raw file**.
3. Guardar los entregables en `Documentos\Taller_Ethical_Hacking\PracticaNN\` con las iniciales del participante en el nombre.
4. **Ética y legalidad:** todas las actividades se limitan a reconocimiento pasivo sobre información pública y a un escaneo simulado en una red ficticia. No acceder a sistemas, servicios o archivos encontrados, no probar credenciales y no escanear redes reales sin autorización escrita del propietario.
5. Las prácticas son progresivas: van del reconocimiento pasivo (Google, Shodan) al reconocimiento activo (Nmap).

## Estructura del repositorio

```text
.
├── README.md            Página principal (este archivo)
├── Setup_Guide.md       Guía de configuración del entorno
├── images/              Logotipo y diagramas de las prácticas
├── Capitulo01/          Práctica 1: README.md y recursos/
├── Capitulo02/          Práctica 2
└── Capitulo03/          Práctica 3
```

## Recursos adicionales

- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)
- [Shodan: Search Query Fundamentals](https://help.shodan.io/the-basics/search-query-fundamentals)
- [Nmap Reference Guide](https://nmap.org/book/man.html)

## Enlaces de referencia

- [Google: refinar búsquedas web](https://support.google.com/websearch/answer/2466433)
- [Google: quitar información de los resultados de búsqueda](https://developers.google.com/search/docs/crawling-indexing/remove-information)
- [Nmap: host de pruebas scanme.nmap.org](http://scanme.nmap.org/)
- [National Vulnerability Database](https://nvd.nist.gov/)

---

## 📬 **Contacto y más información**

Si tienes alguna pregunta o necesitas más detalles, no dudes en [contactarnos](mailto:soporte@netec.com). También puedes encontrar más recursos en nuestra [página](https://netec.com).

---

¡Gracias por visitar nuestra plataforma! No olvides revisar todos los laboratorios y comenzar tu viaje de aprendizaje hoy mismo.
