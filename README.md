

# Cómo Ejecutar docker_n8n: Guía Paso a Paso

![n8n + Docker](https://n8n.io/n8n-logo.png)  
*Automatiza flujos de trabajo con n8n en contenedores Docker*


## 🐳 ¿Qué es este proyecto?

Este repositorio contiene una configuración Docker personalizada para desplegar una instancia de [n8n](https://n8n.io/), una herramienta de automatización de flujos de trabajo de código abierto.


## 🚀 Requisitos

Antes de comenzar, asegúrate de tener instalado:

- [Docker](https://docs.docker.com/get-docker/) (versión 20.10.0 o superior)
- [Docker Compose](https://docs.docker.com/compose/install/) (v2.0.0+)
- Git (opcional pero recomendado)
- 2GB RAM mínimo (4GB recomendado para producción)


## 📦 Contenido

- `docker-compose.yml`: Define los servicios necesarios (n8n, base de datos, etc.).
- `.env`: Variables de entorno configurables.
- `README.md`: Documentación del proyecto.

## ⚙️ Uso

1. Clona este repositorio:

   ```bash
   git clone https://github.com/marangelo/docker_n8n.git
   cd docker_n8n


2. Dentro del archivo `.env` (puedes modificar cada variable ):

   ```bash
   nano .env
   ```

3. Ejecuta los contenedores:

   ```bash
   docker-compose up -d
   ```

4. Accede a n8n en tu navegador:

   ```
   http://localhost:5678
   ```

## 🔐 Seguridad

Este entorno está pensado para desarrollo o pruebas. Para producción, asegúrate de:

* Configurar HTTPS.
* Usar autenticación en n8n.
* No exponer puertos directamente sin un proxy.

## 🛠 Personalización

Puedes modificar las variables en `.env` para cambiar configuración como puertos, credenciales o almacenamiento.

## 📄 Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).

---

> Hecho con ❤️ por [@marangelo](https://github.com/marangelo)
