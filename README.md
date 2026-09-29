# 🍽️ Aroma Restaurant – WebAR Menu

A browser-based Augmented Reality restaurant menu that allows users to explore food items through interactive 3D models and view supported dishes in Augmented Reality.

The project is designed as a lightweight alternative to traditional restaurant menus, combining a responsive web interface with interactive 3D food visualization and WebAR functionality.

---

## 📌 Project Overview

Traditional restaurant menus mainly use text and static photographs to present food items.

This project enhances the menu experience by allowing users to:

- Browse food items by category
- View interactive 3D food models
- Rotate and zoom food models
- View selected food models in Augmented Reality
- Access the menu directly through a web browser
- Use the menu on desktop and supported mobile devices

No dedicated mobile application is required.

---

## 🎯 Objectives

The main objectives of this project are:

- To develop a web-based restaurant menu.
- To integrate interactive 3D food models.
- To implement browser-based Augmented Reality.
- To provide a responsive interface for desktop and mobile devices.
- To organize food items into different categories.
- To demonstrate the practical use of WebAR in the restaurant domain.
- To deploy the project using GitHub Pages.

---

## ✨ Features

### 🍕 Interactive Food Menu

Food items are organized into multiple categories:

- Popular
- Pizza
- Burgers
- Pasta
- Sides
- Desserts

### 🧊 Interactive 3D Models

Users can interact with food models directly in the browser.

Supported interactions include:

- Rotation
- Zoom
- Camera control
- Auto-rotation
- Interactive 3D viewing

### 📱 Augmented Reality

On compatible mobile devices and browsers, users can launch the AR experience and view the selected food model in their physical environment.

AR availability depends on:

- Device hardware
- Operating system
- Browser support
- Camera permissions
- AR framework support

### 📱 Responsive Design

The website is designed to work across:

- Desktop
- Laptop
- Tablet
- Mobile devices

---

## 🍽️ Food Models

The current prototype contains six 3D food models.

| Food Item | Category | Model |
|---|---|---|
| Classic Pizza | Pizza / Popular | `pizza.glb` |
| Classic Burger | Burgers / Popular | `burger.glb` |
| Realistic Burger | Burgers | `burger_realistic_free.glb` |
| Classic Pasta | Pasta / Popular | `pasta_bowl_-_polycam.glb` |
| Crispy French Fries | Sides / Popular | `lifelike_3d_model_of_crispy_french_fries.glb` |
| Classic Donut | Desserts | `donett.glb` |

> **Note:** Prices displayed in the prototype are demonstration values and do not represent actual restaurant prices.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Webpage structure |
| CSS3 | Styling and responsive design |
| JavaScript | Menu interaction and category filtering |
| GLB / glTF | 3D model format |
| Google `<model-viewer>` | Interactive 3D and AR visualization |
| WebXR / AR capabilities | Browser-based AR |
| GitHub | Source code hosting |
| GitHub Pages | Website deployment |

---

## 🏗️ System Architecture

```text
                ┌─────────────────────┐
                │        User         │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    Web Browser      │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │ Restaurant Menu UI  │
                │   HTML + CSS + JS   │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │   <model-viewer>    │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │     GLB Models      │
                └──────────┬──────────┘
                           │
                 ┌─────────┴─────────┐
                 ▼                   ▼
          ┌─────────────┐      ┌─────────────┐
          │ 3D Viewer   │      │     AR      │
          └─────────────┘      └─────────────┘
