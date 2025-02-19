Aquí tienes un **README.md** profesional y bien estructurado para tu proyecto en **Docker + FastAPI**. 🚀  

---

### 📌 **README.md - FastAPI con Docker**  

```markdown
# FastAPI + Docker 🚀

Este repositorio contiene una aplicación web construida con **FastAPI**, empaquetada y desplegable con **Docker**.

---

## 📖 **Índice**
1. [Requisitos](#requisitos)
2. [Instalación](#instalación)
3. [Construcción de la Imagen Docker](#construcción-de-la-imagen-docker)
4. [Ejecución del Contenedor](#ejecución-del-contenedor)
5. [Acceso a la API](#acceso-a-la-api)
6. [Publicación en Docker Hub](#publicación-en-docker-hub)
7. [Gestión y Limpieza de Contenedores](#gestión-y-limpieza-de-contenedores)
8. [Licencia](#licencia)

---

## ✅ **Requisitos**
Antes de comenzar, asegúrate de tener instalados los siguientes componentes en tu sistema:

- [Python 3.9+](https://www.python.org/downloads/)
- [Docker](https://www.docker.com/get-started)
- [Git](https://git-scm.com/)

Para verificar que Docker está instalado correctamente, ejecuta:

```bash
docker --version
```

---

## ⚙️ **Instalación**
Clona este repositorio en tu máquina local:

```bash
git clone https://github.com/bryan_percy/fastapi-docker.git
cd fastapi-docker
```

Si deseas trabajar en un entorno virtual de Python, ejecútalo:

```bash
python -m venv venv
source venv/bin/activate  # En Windows usa: venv\Scripts\activate
pip install -r requirements.txt
```

---

## 🛠 **Construcción de la Imagen Docker**
Para construir la imagen Docker, ejecuta el siguiente comando en la raíz del proyecto:

```bash
docker build -t bryan_percy/fastapi-app:v1 .
```

Este comando crea una imagen basada en el `Dockerfile` del proyecto y la etiqueta con `v1`.

---

## 🚀 **Ejecución del Contenedor**
Para iniciar un contenedor basado en la imagen creada, usa:

```bash
docker run -d -p 8000:8000 --name fastapi-container bryan_percy/fastapi-app:v1
```

- `-d`: Ejecuta el contenedor en segundo plano.
- `-p 8000:8000`: Mapea el puerto 8000 del contenedor al 8000 de la máquina.
- `--name fastapi-container`: Asigna un nombre al contenedor.

---

## 🌍 **Acceso a la API**
Una vez que el contenedor esté en ejecución, abre tu navegador y accede a:

🔹 **Interfaz principal**  
[http://localhost:8000](http://localhost:8000)

🔹 **Documentación interactiva de la API (Swagger UI)**  
[http://localhost:8000/docs](http://localhost:8000/docs)

🔹 **Alternativa de documentación (Redoc UI)**  
[http://localhost:8000/redoc](http://localhost:8000/redoc)

---

## 📤 **Publicación en Docker Hub**
Para subir la imagen a Docker Hub, sigue estos pasos:

1. **Inicia sesión en Docker Hub**:

   ```bash
   docker login
   ```

2. **Etiqueta la imagen con el formato adecuado**:

   ```bash
   docker tag bryan_percy/fastapi-app:v1 bryan_percy/fastapi-app:latest
   ```

3. **Sube la imagen al repositorio de Docker Hub**:

   ```bash
   docker push bryan_percy/fastapi-app:latest
   ```

4. **Verifica la imagen en Docker Hub**:  
   Visita [https://hub.docker.com/r/bryan_percy/fastapi-app](https://hub.docker.com/r/bryan_percy/fastapi-app) para confirmar la subida.

---

## 🗑 **Gestión y Limpieza de Contenedores**
### 📌 **Listar los contenedores en ejecución**
```bash
docker ps
```

### 📌 **Detener un contenedor en ejecución**
```bash
docker stop fastapi-container
```

### 📌 **Eliminar un contenedor detenido**
```bash
docker rm fastapi-container
```

### 📌 **Eliminar una imagen Docker innecesaria**
```bash
docker rmi bryan_percy/fastapi-app:latest
```

### 📌 **Liberar espacio eliminando todos los contenedores detenidos**
```bash
docker container prune
```

---

## 📜 **Licencia**
Este proyecto está bajo la **Licencia MIT**. Consulta el archivo `LICENSE` para más detalles.

---

## 🛠 **Autor**
👤 **Bryan Percy**  
📧 Contacto: [bryanpercy77@gmail.com](mailto:bryanpercy77@gmail.com)  
🔗 GitHub: [github.com/bryan_percy](https://github.com/bryan_percy)

---

### 🚀 ¡Listo para
