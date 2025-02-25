# Crezco Donation App

Este repositorio alberga una colección de librerías desarrolladas en **Angular** para gestionar las donaciones de **Crezco Foundation**. Inicialmente, se ha desarrollado la librería [`crezco-donation-app`](https://github.com/CrezcoFoundation/crezco-donation-app) que integra **Stripe** como método de pago. Sin embargo, el objetivo es expandir la compatibilidad con otros medios de donación como **PayPal**, **Cash App**, y otros.

## 📌 Objetivo

Facilitar la integración de múltiples métodos de pago en las plataformas de donación de **Crezco Foundation**, proporcionando componentes y servicios reutilizables dentro del ecosistema **Angular**.

## 🚀 Librerías Planeadas

### 1. [`crezco-donation-app`](https://github.com/CrezcoFoundation/crezco-donation-app)
   - Maneja pagos a través de **Stripe**.
   - Implementa un formulario paso a paso para donaciones únicas y recurrentes.
   - Utiliza la API de **PaymentIntents** y **SetupIntents** de Stripe.
   - Gestiona el estado con **NgRx**.

### 2. `crezco-donation-paypal` *(en desarrollo)*
   - Implementación de donaciones vía **PayPal Checkout**.
   - Soporte para pagos únicos y suscripciones.

### 3. `crezco-donation-cashapp` *(planeado)*
   - Integración con **Cash App Pay** para donaciones instantáneas.

## 🛠 Tecnologías Utilizadas

- **Angular** (Framework principal)
- **NgRx** (Gestión de estado)
- **Bootstrap 5** (Diseño de formularios y UI)
- **Stripe API** (Para procesamiento de pagos en `crezco-donation-app`)
- **PayPal API** *(en desarrollo)*
- **Cash App API** *(planeado)*

## 📄 Estructura del Repositorio

Cada librería se desarrolla como un paquete independiente dentro del monorepo, siguiendo la estructura recomendada para librerías en Angular:

```
crezco-donation-app/
│── projects/
│   ├── crezco-donation-app/       # Integración con Stripe
│   ├── crezco-donation-paypal/     # Integración con PayPal (en desarrollo)
│   ├── crezco-donation-cashapp/    # Integración con Cash App (planeado)
│── angular.json
│── package.json
│── README.md
```

## 📦 Instalación y Uso

Cada librería se publica como un paquete independiente en **npm**. Para usar una de ellas en un proyecto de Angular, puedes instalarla con:

```sh
npm install @crezco-foundation/crezco-donation-app
```

Luego, importa los módulos y servicios necesarios en tu aplicación Angular.

## 🚀 Desarrollo

### Servidor de Desarrollo

Ejecuta el siguiente comando para iniciar un servidor local de desarrollo:
```sh
ng serve
```
Luego, navega a `http://localhost:4200/`. La aplicación se recargará automáticamente cuando realices cambios en los archivos fuente.

### Generación de Código

Ejecuta:
```sh
ng generate component nombre-componente
```
Para generar un nuevo componente. También puedes usar `ng generate directive|pipe|service|class|guard|interface|enum|module`.

### Construcción del Proyecto

Ejecuta:
```sh
ng build
```
El resultado se almacenará en la carpeta `dist/`.

### Pruebas Unitarias

Ejecuta:
```sh
ng test
```
Para ejecutar las pruebas unitarias con **Karma**.

### Pruebas End-to-End

Ejecuta:
```sh
ng e2e
```
Para ejecutar pruebas de extremo a extremo (E2E). Antes de ejecutar este comando, asegúrate de agregar un paquete que implemente esta capacidad.

## 📚 Contribución

Si deseas contribuir al desarrollo de las librerías, sigue estos pasos:

1. **Clona el repositorio:**
   ```sh
   git clone https://github.com/CrezcoFoundation/crezco-donation-app.git
   ```
2. **Instala dependencias:**
   ```sh
   npm install
   ```
3. **Selecciona la librería en la que trabajar:**
   ```sh
   cd projects/crezco-donation-app
   ```
4. **Levanta el entorno de desarrollo:**
   ```sh
   ng serve
   ```
5. **Envía un Pull Request con tus cambios.**

## 📬 Contacto

Si tienes preguntas o sugerencias, por favor, abre un **issue** en este repositorio o contacta al equipo de Crezco Foundation.

---
🚀 **Crezco Foundation** – Facilitando donaciones a través de tecnología.
