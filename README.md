# 🐳 Docker

**Descripción:** Este documento constituye un apunte técnico recopilatorio de los conceptos fundamentales y operativos de Docker.

El objetivo es brindar una guía estructurada sobre la gestión de imágenes, contenedores, persistencia de datos (volúmenes), redes y automatización mediante *Dockerfiles*, bajo un enfoque práctico y académico.

> 🚧 Resta agregar un par de secciones más.

---

## 🗂️ Estructura del Repositorio
```text
├── 1. Post-Instalación
│   ├── 1.Chequear_versión.md
│   └── 3.Logueo.md
├── 2. Imágenes & Contenedores
│   ├── 1.Traer_Imágenes.md
│   ├── 2.Crear_Contenedor.md
│   ├── 3.Detener_Contenedor.md
│   └── 4.Contenedores_Múltiples.md
├── 3. Volúmenes
│   ├── 1.Crear_Volúmen.md
│   ├── 2.Montar_Volúmen.md
│   ├── 3.Persistir_Datos.md
│   ├── 4.Eliminar_Volúmen.md
│   └── 5.Limpieza.md
├── 4. Ejecución
│   ├── 1.Exec.md
│   └── 2.Shell Interactiva.md
├── 5. Network
│   ├── 1.Eliminar_Red.md
│   ├── 2.Aislamiento.md
│   ├── 3.Teoría_Load_Balancers.md
│   ├── 4.Servidor_de_Prueba.md
│   ├── 5.Bridge.md
│   └── 6.Práctica_Load_Balancers.md
├── 6. Dockerfiles
│   ├── 1.Crear_Dockerfile.md
│   ├── 2.Contenerizar-1.md
│   ├── 3.Contenerizar-2.md
│   ├── 4.Variables_de_Entorno.md
│   ├── 5.Dockerizando.md
│   ├── 6.Errores.md
│   └── 7.Soluciones.md
└── README.md
```

---

## 📘 Contenido

### 🔧 1. Post-Instalación
> Protocolos de validación del *daemon* y autenticación mediante CLI.

| Archivo | Descripción |
| :--- | :--- |
| `1.Chequear_versión.md` | Diagnóstico de compatibilidad entre cliente y servidor. |
| `3.Logueo.md` | Mecanismos de autenticación en repositorios de contenedores. |

### 📦 2. Imágenes & Contenedores
> Gestión del ciclo de vida y abstracción de entornos.

| Archivo | Descripción |
| :--- | :--- |
| `1.Traer_Imágenes.md` | Operaciones de *pulling* y auditoría de caché local. |
| `2.Crear_Contenedor.md` | Instanciación de contenedores y mapeo de puertos (*forwarding*). |
| `3.Detener_Contenedor.md` | Gestión ordenada (*SIGTERM*) vs. forzada (*SIGKILL*) de procesos. |
| `4.Contenedores_Múltiples.md` | Escalabilidad horizontal mediante instancias aisladas en puertos distintos. |

### 💾 3. Volúmenes
> Estrategias de persistencia de datos fuera del ciclo de vida del contenedor.

| Archivo | Descripción |
| :--- | :--- |
| `1.Crear_Volúmen.md` | Aproximación teórica y operativa a la gestión de volúmenes persistentes. |
| `2.Montar_Volúmen.md` | Implementación práctica de persistencia en aplicaciones CMS (*Ghost*). |
| `3.Persistir_Datos.md` | Validación de la integridad de datos tras la eliminación del contenedor. |
| `4.Eliminar_Volúmen.md` | Gestión del ciclo de vida y limpieza de recursos bloqueados. |
| `5.Limpieza.md` | Procedimientos de saneamiento integral del sistema Docker. |

### ⚙️ 4. Ejecución
> Interacción con procesos en ejecución y acceso a *shells*.

| Archivo | Descripción |
| :--- | :--- |
| `1.Exec.md` | Ejecución de comandos no interactivos dentro de contenedores activos. |
| `2.Shell Interactiva.md` | Acceso a *TTY* para depuración y manipulación *in-situ*. |

### 🌐 5. Network
> Topologías de red y balanceo de carga.

| Archivo | Descripción |
| :--- | :--- |
| `1.Eliminar_Red.md` | Implementación de aislamiento absoluto mediante `--network none`. |
| `2.Aislamiento.md` | Validación empírica de la desconexión total del stack de red. |
| `3.Teoría_Load_Balancers.md` | Fundamentos teóricos: *Round Robin*, *Least Connections*, *Proxy Reverso*. |
| `4.Servidor_de_Prueba.md` | Configuración de entornos de servidores (*Caddy*) para balanceo. |
| `5.Bridge.md` | Redes personalizadas y resolución de nombres mediante *DNS* interno. |
| `6.Práctica_Load_Balancers.md` | Implementación de balanceo de carga distribuido (*round-robin*). |

### 🏗️ 6. Dockerfiles
> Infraestructura como Código (*IaC*): automatización y construcción.

| Archivo | Descripción |
| :--- | :--- |
| `1.Crear_Dockerfile.md` | Definición inmutable de entornos mediante *Dockerfile*. |
| `2.Contenerizar-1.md` | Preparación y compilación de binarios para despliegue. |
| `3.Contenerizar-2.md` | Empaquetado de artefactos compilados en imágenes base ligeras (*slim*). |
| `4.Variables_de_Entorno.md` | Configuración dinámica mediante el uso de directivas `ENV`. |
| `5.Dockerizando.md` | Automatización de flujos de trabajo basados en *Python*. |
| `6.Errores.md` | Análisis de fallos de tiempo de ejecución por dependencias faltantes. |
| `7.Soluciones.md` | Resolución de dependencias y optimización del *build*. |

---

