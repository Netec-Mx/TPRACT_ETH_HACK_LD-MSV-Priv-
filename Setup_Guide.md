<img src="images/neteclogo.png" alt="logo" width="300"/>

# Setup Guide General

## Introducción al Ethical Hacking

| Control documental | Información |
|---|---|
| Clave del curso | TPRACT_ETH_HACK_LD MSV (Priv) |
| Versión del documento | 1.0 |
| Estado | BORRADOR: revisión documental completa; pendiente de validación con cuentas de participante |
| Instructor responsable | Por asignar por Netec |
| Fecha de elaboración | 2026-11-10 |
| Fecha de última validación | 2026-11-10 (revisión de herramientas y enlaces) |
| Repositorio de laboratorios | Repositorio de GitHub de Netec del curso (rama `main`) |
| Rama y revisión analizada | `main`, versión 1.0 |
| Alcance revisado | 1 capítulo, 3 prácticas, 4 archivos de recursos, README principal y Setup Guide |
| Modalidad del entorno | Web (servicios gratuitos); Nmap en entorno simulado con Google AI Studio |

[Inicio](README.md)

# Objetivo

Preparar, para cada participante, un equipo con navegador actualizado, un editor de hojas de cálculo, una cuenta de Google con acceso a Google AI Studio y una cuenta gratuita de Shodan. El entorno se considera listo cuando se aprueban las validaciones de la sección [Validación del Entorno](#validacion-entorno). Los participantes no instalan Nmap: la Práctica 3 usa un simulador. Solo el instructor, de forma opcional, necesita Nmap para una demostración autorizada.

# Requisitos de Hardware

| Recurso | Mínimo requerido | Recomendado | Observaciones |
|---|---|---|---|
| Equipo | Laptop o PC de 64 bits, 2 núcleos | 4 núcleos | Todas las herramientas de los participantes son web |
| Memoria RAM | 4 GB | 8 GB | Varias pestañas abiertas |
| Espacio libre | 1 GB | 2 GB | Los recursos ocupan menos de 1 MB |
| Pantalla | 1366 × 768 | 1920 × 1080 | Facilita trabajar con el navegador y la matriz a la vez |
| Conectividad | 5 Mbps | 10 Mbps | Acceso HTTPS a los sitios de la sección [Servicios Externos Requeridos](#servicios-externos) |

# Sistemas Operativos Compatibles

| Sistema operativo | Edición y versión | Arquitectura | Condición de soporte o validación |
|---|---|---|---|
| Windows | 10 u 11 | x64 | Plataforma base; compatible según fabricante; pendiente de validar con cuenta de participante |
| macOS | 13 o posterior | Apple silicon o Intel | Compatible según fabricante; no validado |
| Linux | Distribución con navegador actualizado | x64 | Compatible según fabricante; no validado |

# Software Requerido

| Componente | Edición y versión requerida | Arquitectura | Obligatorio u opcional | Fuente oficial |
|---|---|---|---|---|
| Navegador Google Chrome o Microsoft Edge | Versión estable vigente | x64 | Obligatorio | [google.com/chrome](https://www.google.com/chrome/) |
| Editor de hojas de cálculo | Microsoft Excel (escritorio o web), Google Sheets o LibreOffice Calc | x64 | Obligatorio | [microsoft365.com](https://www.microsoft365.com/) o [libreoffice.org](https://www.libreoffice.org/download/download-libreoffice/) |
| Google Search | Servicio público | N/A | Obligatorio (Práctica 1) | [google.com](https://www.google.com/) |
| Shodan | Servicio administrado, cuenta gratuita | N/A | Obligatorio (Práctica 2) | [shodan.io](https://www.shodan.io/) |
| Google AI Studio | Servicio administrado, nivel gratuito | N/A | Obligatorio (Práctica 3) | [aistudio.google.com](https://aistudio.google.com/) |
| Nmap | 7.95 o la versión estable vigente | x64 | Opcional, solo equipo del instructor (demostración de la Práctica 3) | [nmap.org/download](https://nmap.org/download.html) |

# Herramientas y Dependencias

## Paquetes, frameworks y componentes adicionales

| Dependencia | Versión o restricción | Componente que la necesita | Método de instalación o habilitación |
|---|---|---|---|
| Simulador de Nmap | Instrucciones de sistema del repositorio | Práctica 3 | Pegar `Capitulo03/recursos/Simulador_Nmap_Instrucciones.txt` en **System instructions** de Google AI Studio |
| Plantillas de entregables | Versión 1.0 del repositorio | Prácticas 1 a 3 | Carpetas `CapituloNN/recursos/` |

## Licencias, cuentas y permisos

| Recurso o servicio | Licencia o suscripción | Cuenta o rol requerido | Permiso mínimo | Responsable de habilitación |
|---|---|---|---|---|
| Shodan | Gratuita | Cuenta de Shodan con correo personal | Usuario | Cada participante (antes del taller) |
| Google AI Studio | Gratuita | Cuenta de Google (mayor de edad, región con servicio disponible) | Usuario | Cada participante |
| Google Hacking Database | Acceso público | Sin cuenta | Lectura | No aplica |
| Autorización de la demostración de Nmap | Uso permitido por el proyecto Nmap para `scanme.nmap.org` | Instructor | Escaneo moderado | Instructor |

No registrar contraseñas en el repositorio ni en los entregables.

# Instalación y Configuración

## 1. Obtener los materiales

- Repositorio autorizado: repositorio de GitHub del curso (botón **Code > Download ZIP**) o paquete ZIP del instructor.
- Revisión: rama `main`.
- Directorio de trabajo: `Documentos\Taller_Ethical_Hacking\` con las subcarpetas `Practica01` a `Practica03`.

## 2. Instalar o habilitar los componentes

### Cuenta de Shodan

1. Abrir [shodan.io](https://www.shodan.io/) y seleccionar **Login** > **Create an Account**.
2. Confirmar la cuenta desde el correo recibido.
3. Buscar `scanme.nmap.org`.

**Resultado esperado:** la búsqueda muestra el host 45.33.32.156.

### Google AI Studio

1. Iniciar sesión en [aistudio.google.com](https://aistudio.google.com/) y aceptar los términos si aparecen.
2. Abrir un chat nuevo y enviar *"Responde solo OK"*.

**Resultado esperado:** el modelo responde OK.

### Nmap (solo instructor, opcional)

1. Descargar e instalar Nmap desde [nmap.org/download](https://nmap.org/download.html).
2. Ejecutar en una terminal:

```bash
nmap --version
```

**Resultado esperado:** la versión de Nmap instalada. Para la demostración se usa únicamente `nmap -sV scanme.nmap.org`.

### Carpetas de trabajo

1. Crear `Documentos\Taller_Ethical_Hacking\` y, dentro, `Practica01` a `Practica03`.
2. Copiar a cada carpeta el contenido de `CapituloNN\recursos`.

## 3. Preparar archivos de configuración

No se requieren archivos de configuración.

# Variables de Entorno

No se requieren variables de entorno.

# Configuración Base para los Laboratorios

## Parámetros comunes

| Parámetro | Valor o convención | Observaciones |
|---|---|---|
| Raíz de trabajo | `Documentos\Taller_Ethical_Hacking\` | Una carpeta por práctica |
| Nombre de entregables | `Nombre_[INICIALES].xlsx` | Iniciales del participante |
| Sitio de prueba para dorks | `testfire.net` | Aplicación de demostración de IBM para pruebas de seguridad |
| Host autorizado para análisis | `scanme.nmap.org` (45.33.32.156) | Publicado por el proyecto Nmap para pruebas |
| Red simulada | `10.10.10.0/24` | Definida en las instrucciones del simulador |

## Estructura de carpetas

```text
Documentos\Taller_Ethical_Hacking\
├── Practica01\ ... Practica03\   Recursos y entregables de cada práctica
```

## Recursos compartidos

No hay recursos compartidos entre participantes.

## Preparación antes de cada práctica

| Práctica | Preparación |
|---|---|
| 1 | Leer las reglas éticas; tener abierta la matriz de dorks |
| 2 | Sesión iniciada en Shodan |
| 3 | Sesión iniciada en Google AI Studio; el instructor prepara (opcional) la demostración con Nmap |

## Correcciones de coherencia

| Inconsistencia o dependencia omitida | Configuración unificada | Ajuste necesario en las copias de trabajo |
|---|---|---|
| El temario indica "Nmap en entorno simulado con Google AI Studio" sin definir el entorno | Instrucciones de sistema con una red de laboratorio fija (`10.10.10.0/24`, 6 hosts) en `Capitulo03/recursos` | Ninguno |
| El Google Dorking puede revelar información de organizaciones reales | Dorks sobre sitios públicos y un sitio de prueba autorizado, con reglas éticas explícitas | Ninguno |
| El temario agrupa las 3 prácticas en el Capítulo 1 | Una carpeta `CapituloNN` por práctica, según la estructura de laboratorios de Netec | Ninguno |

# Servicios Externos Requeridos <a id="servicios-externos"></a>

| Servicio | URL, endpoint o región | Uso | Acceso requerido |
|---|---|---|---|
| Google Search | [google.com](https://www.google.com/) | Práctica 1 | Público |
| Google Hacking Database | [exploit-db.com/google-hacking-database](https://www.exploit-db.com/google-hacking-database) | Práctica 1 | Público |
| Shodan | [shodan.io](https://www.shodan.io/) | Práctica 2 | Cuenta gratuita |
| Google AI Studio | [aistudio.google.com](https://aistudio.google.com/) | Práctica 3 | Cuenta de Google |
| GitHub | [github.com](https://github.com/) | Descarga de materiales | Lectura del repositorio |

## Configuración de red

| Origen | Destino | Protocolo y puerto | Sentido | Condición |
|---|---|---|---|---|
| Equipo del participante | google.com, exploit-db.com, shodan.io, aistudio.google.com, github.com | HTTPS 443 | Saliente | Dominios permitidos en el proxy o firewall |
| Equipo del instructor (opcional) | scanme.nmap.org | TCP a puertos de servicio | Saliente | Solo para la demostración; algunas redes corporativas bloquean escaneos |

# Creación de Entornos / Máquinas Virtuales / Emuladores

| Elemento | Tipo o plataforma | Imagen y versión | Recursos asignados | Red o región | Persistencia |
|---|---|---|---|---|---|
| Simulador de Nmap | Chat de Google AI Studio con instrucciones de sistema | Modelo vigente de Google AI Studio | No aplica | Red ficticia `10.10.10.0/24` | El chat puede guardarse en la cuenta de Google |

1. Abrir un chat nuevo en Google AI Studio.
2. Pegar el contenido de `Simulador_Nmap_Instrucciones.txt` en **System instructions**.
3. Bajar **Temperature** a `0` o al mínimo.
4. Enviar `nmap -sn 10.10.10.0/24` y comprobar que aparecen 6 hosts activos.

<a id="validacion-entorno"></a>

# Validación del Entorno

| ID | Componente o capacidad | Procedimiento | Resultado esperado | Evidencia mínima |
|---|---|---|---|---|
| V-01 | Materiales | Abrir `Capitulo01/recursos/Matriz_Google_Dorks.xlsx` | La matriz se abre y tiene 3 hojas | Captura |
| V-02 | Google Search | Buscar `site:nmap.org filetype:pdf` | Resultados en PDF de nmap.org | Captura |
| V-03 | Shodan | Iniciar sesión y buscar `scanme.nmap.org` | Aparece el host 45.33.32.156 | Captura |
| V-04 | Shodan (filtros) | Buscar `port:22 country:MX` | Total de resultados y resúmenes | Captura |
| V-05 | Simulador de Nmap | Configurar el simulador y enviar `nmap -sn 10.10.10.0/24` | 6 hosts activos | Captura |

**Criterio de entorno listo:** V-01 a V-05 aprobadas.

# Comandos de Verificación

## Nmap (solo instructor, opcional)

**Plataforma y terminal:** Windows (PowerShell), macOS o Linux (terminal).
**Directorio de ejecución:** cualquiera.
**Prerrequisito:** Nmap instalado y red que permita el escaneo.

```bash
nmap -sV scanme.nmap.org
```

**Resultado esperado:**

```text
PORT     STATE SERVICE VERSION
22/tcp   open  ssh     OpenSSH 6.6.1p1 Ubuntu 2ubuntu2.13
80/tcp   open  http    Apache httpd 2.4.7 ((Ubuntu))
```

**Interpretación:** confirma que la demostración puede realizarse. Los puertos y versiones pueden cambiar si el proyecto Nmap actualiza el servidor.

# Troubleshooting

| Síntoma | Causa probable | Comprobación | Corrección | Validación posterior |
|---|---|---|---|---|
| Google muestra CAPTCHA | Muchas búsquedas desde la misma red | Mensaje en pantalla | Resolver manualmente y esperar entre búsquedas | V-02 |
| Shodan pide membresía | Filtro o volumen no incluido en la cuenta gratuita | Mensaje de Shodan | Usar la consulta alternativa de la práctica | V-04 |
| El simulador no responde como Nmap | Instrucciones fuera de **System instructions** | Revisar el panel | Pegar las instrucciones en el campo correcto e iniciar un chat nuevo | V-05 |
| Google AI Studio no está disponible | Restricción de edad, región o cuenta administrada | Mensaje al iniciar sesión | Usar una cuenta de Google personal o trabajar en pareja | V-05 |

# Checklist Final

- [ ] Navegador actualizado y editor de hojas de cálculo funcional.
- [ ] Cuenta de Shodan creada y confirmada.
- [ ] Cuenta de Google con acceso a Google AI Studio.
- [ ] Recursos descargados en `Documentos\Taller_Ethical_Hacking\`.
- [ ] Validaciones V-01 a V-05 aprobadas.

# Resumen

Para iniciar el taller, cada participante necesita un navegador actualizado, un editor de hojas de cálculo, una cuenta gratuita de Shodan y una cuenta de Google con acceso a Google AI Studio. No se instala software en los equipos de los participantes; Nmap solo es opcional para la demostración del instructor.

<a id="registro-validacion"></a>

## Registro de validación

| Fecha | Responsable | Plataforma o entorno probado | Resultado | Limitaciones o acciones pendientes |
|---|---|---|---|---|
| 2026-11-10 | Desarrollo de contenido Netec | Revisión de enlaces y herramientas: Google Hacking Database, ficha de 45.33.32.156 en Shodan, documentación de Nmap | APTO para publicación del repositorio | No se ejecutó el simulador de Nmap con cuenta de participante. Pendiente: V-01 a V-05 |

## Referencias oficiales

| Documento o recurso | URL | Fecha de consulta |
|---|---|---|
| Google: refinar búsquedas web | https://support.google.com/websearch/answer/2466433 | 2026-11-10 |
| Google Hacking Database | https://www.exploit-db.com/google-hacking-database | 2026-11-10 |
| Shodan: Search Query Fundamentals | https://help.shodan.io/the-basics/search-query-fundamentals | 2026-11-10 |
| Nmap Reference Guide | https://nmap.org/book/man.html | 2026-11-10 |
| Nmap: scanme.nmap.org | http://scanme.nmap.org/ | 2026-11-10 |
| Google AI Studio | https://aistudio.google.com/ | 2026-11-10 |

[Inicio](README.md)
