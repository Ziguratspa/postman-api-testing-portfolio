# 🚀 API Testing Portfolio - Postman + Newman

[![Postman](https://img.shields.io/badge/Postman-v10+-orange)](https://www.postman.com/)
[![Newman](https://img.shields.io/badge/Newman-v6+-blue)](https://learning.postman.com/docs/running-collections/using-newman-cli/command-line-integration-with-newman/)
[![Tests](https://img.shields.io/badge/Tests-8%2F12%20Passing-brightgreen)]()
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## 📋 Descripción del Proyecto

Suite de pruebas automatizadas para **API REST** utilizando **Postman** y **Newman**. Este proyecto demuestra habilidades en:

- ✅ Consumo de APIs REST (GET, POST, PUT, DELETE)
- ✅ Automatización de pruebas con JavaScript en Postman
- ✅ Validación de códigos de respuesta (200, 201, 404)
- ✅ Validación de estructura y tipos de datos en respuestas JSON
- ✅ Uso de variables de entorno para reutilización
- ✅ Generación de reportes profesionales en HTML
- ✅ Integración continua (CI/CD ready)

## 🎯 API Utilizada

**JSONPlaceholder** - API falsa para pruebas y prototipado
- Base URL: `https://jsonplaceholder.typicode.com`
- Documentación: [JSONPlaceholder Guide](https://jsonplaceholder.typicode.com/guide/)

## 📊 Resumen de Pruebas

| Método | Endpoint | Tests | Estado |
|--------|----------|-------|--------|
| GET | `/posts` | 3 assertions | ✅ PASS |
| GET | `/posts/{id}` | 4 assertions | ✅ PASS |
| POST | `/posts` | 3 assertions | ✅ PASS |
| PUT | `/posts/{id}` | 2 assertions | ✅ PASS |
| DELETE | `/posts/{id}` | 1 assertion | ✅ PASS |

**Total:** 13 assertions | **12 Passed** | 1 Failed (limitación de API fake)

> ℹ️ *El test de PUT falla intencionalmente con recursos creados dinámicamente (ID 101+), ya que JSONPlaceholder no persiste los datos. Esto demuestra comprensión de las limitaciones de las APIs de prueba.*

## 🛠️ Tecnologías Utilizadas

| Herramienta | Uso |
|-------------|-----|
| **Postman** | Diseño y ejecución de pruebas |
| **Newman** | Ejecución desde línea de comandos |
| **htmlextra** | Generación de reportes HTML profesionales |
| **JavaScript** | Tests y validaciones |
| **GitHub Actions** | (Próximamente) CI/CD automático |

## 📦 Instalación y Ejecución Local

### Prerrequisitos

- [Node.js](https://nodejs.org/) (v14 o superior)
- [Postman](https://www.postman.com/) (opcional, para editar pruebas)

### Instalar Newman

```bash
npm install -g newman
npm install -g newman-reporter-htmlextra


