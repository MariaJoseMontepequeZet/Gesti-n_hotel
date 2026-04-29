# Hotel Management System - JavaScript Asynchronous Logic

![JavaScript](https://img.shields.io/badge/Language-JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Academic_Project-blue)

Sistema de gestión hotelera diseñado para ejecutar operaciones CRUD en memoria, aplicando conceptos avanzados de **asincronía clásica** en JavaScript. Este proyecto simula la latencia de procesos de backend mediante el uso controlado de la pila de llamadas (Call Stack) y el Event Loop.

> Hecho por **María José Montepeque Zet**

## 📋 Tabla de Contenidos
1. [Descripción](#descripción)
2. [Arquitectura de Software](#arquitectura-de-software)
3. [Flujo Asíncrono](#flujo-asíncrono)
4. [Instalación y Uso](#instalación-y-uso)
5. [Estructura del Proyecto](#estructura-del-proyecto)

## 📖 Descripción
La aplicación permite administrar habitaciones, huéspedes y estados de limpieza. A diferencia de las implementaciones modernas, este sistema utiliza **callbacks de retorno** para manejar el flujo del programa, garantizando que el hilo principal no se bloquee durante las simulaciones de espera.

## 🏗️ Arquitectura de Software

### Modelo de Datos
Se utiliza un almacenamiento centralizado en un arreglo de objetos, donde cada entidad `habitación` mantiene la siguiente integridad:
* **Precisión Numérica:** Los costos se calculan y muestran con un estándar de **4 decimales**.
* **Gestión de Estados:** Lógica condicional para estados de *Libre*, *Ocupada* y *Limpieza*.

### Flujo Asíncrono (Callback Pattern)
Para cumplir con los requerimientos técnicos, se implementó un patrón de **Recursividad Asíncrona**. El menú principal se pasa como una referencia funcional a los procesos con `setTimeout`, permitiendo que la interfaz de usuario (`prompt`) se reactive solo cuando la "operación de base de datos" ha finalizado.

## 🛠️ Tecnologías y Estándares
* **Vanilla JavaScript (ES6+)**
* **Funciones de Orden Superior:** `.find()`, `.findIndex()`, `.forEach()`, `.splice()`.
* **Control de Versiones:** Desarrollado bajo metodología **Gitflow** para una gestión de ramas limpia y organizada.

## 🚀 Instalación y Uso

1. **Clonar el repositorio:**
   ```bash
   git clone (https://github.com/MariaJoseMontepequeZet/Gesti-n_hotel)