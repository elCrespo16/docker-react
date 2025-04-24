---

# React App - Práctica con Docker y Kubernetes

Este repositorio contiene una aplicación sencilla de **React**, diseñada específicamente como material de práctica para el curso de Udemy:
**[Docker and Kubernetes: The Complete Guide](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/)**, impartido por **Stephen Grider**.

## 📚 Sobre el curso

Este curso enseña cómo construir, empaquetar y desplegar aplicaciones modernas utilizando Docker y Kubernetes. A lo largo del curso, se crean distintas aplicaciones (principalmente en React y Node.js) que luego se dockerizan y se despliegan en distintos entornos, incluyendo clusters de Kubernetes.

## 🚀 Objetivo del repositorio

Este proyecto tiene como objetivo servir de base para:

- Aprender a crear imágenes Docker a partir de una app React.
- Usar `docker-compose` para gestionar múltiples servicios (si aplica).
- Implementar despliegues en Kubernetes.
- Entender cómo manejar rutas, volúmenes, servicios y pods.

## 🛠️ Tecnologías utilizadas

- **React** (frontend)
- **Docker**
- **Docker Compose**
- **Kubernetes (kubectl, minikube, etc.)**
- (Opcionalmente) **Node.js**, si se agrega un backend en fases posteriores.

## 📦 Estructura del proyecto

```
/react-app         # Código fuente de la aplicación React
/Dockerfile        # Instrucciones para construir la imagen Docker de React
/docker-compose.yml (opcional)
/k8s               # Archivos de configuración de Kubernetes (si aplica)
/README.md         # Este archivo
```

## ⚙️ Cómo usar este repositorio

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
```

### 2. Instalar dependencias

```bash
cd react-app
npm install
```

### 3. Ejecutar en desarrollo (sin Docker)

```bash
npm start
```

### 4. Construir y correr con Docker

```bash
docker build -t react-app .
docker run -p 3000:3000 react-app
```

### 5. Usar docker-compose (si has configurado uno)

```bash
docker-compose up
```

### 6. Desplegar en Kubernetes (si has creado los manifiestos)

```bash
kubectl apply -f k8s/
```

> Nota: Asegúrate de tener un cluster corriendo (como minikube) antes de aplicar configuraciones de Kubernetes.

## ✅ Estado del proyecto

Este proyecto está en curso y se irá actualizando según avance en el curso. La idea es que cada etapa (Docker, docker-compose, Kubernetes) se refleje en diferentes ramas o commits del repositorio.

## ✍️ Autor

Este proyecto fue creado como parte del aprendizaje personal del curso de Docker y Kubernetes.
Si tienes sugerencias, mejoras o quieres colaborar, ¡bienvenido!