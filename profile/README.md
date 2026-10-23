<div align="center">

# Panify

### *"Horneamos Calidad, Entregamos Confianza y Unimos Lazos."*

![SENA](https://img.shields.io/badge/SENA-ADSO-39A900?style=for-the-badge)
![Ficha](https://img.shields.io/badge/Ficha-3315796-blue?style=for-the-badge)
![Grupo](https://img.shields.io/badge/Grupo-4-orange?style=for-the-badge)

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

</div>

---

## 📌 Sobre el proyecto

**Panify** es una solución web de gestión operativa y logística diseñada para la fábrica de pan **Distribuciones Oro Pan**. El sistema centraliza y automatiza el ciclo completo del negocio: desde el catálogo de productos y el control de existencias en tiempo real, hasta la recepción de pedidos, la generación de recibos digitales y la coordinación de rutas de entrega.

> 🎓 Proyecto formativo desarrollado en el programa de **Análisis y Desarrollo de Software (ADSO)** del **SENA** — Ficha 3315796, Grupo 4.

---

## 📂 Repositorios de la organización

| Repositorio | Descripción | Stack principal |
| :--- | :--- | :--- |
| [🎨 **Panify-Frontend**](https://github.com/Panify-HQ/Panify-Frontend) | Aplicación web cliente con interfaz responsiva (*Mobile First*) y paneles adaptativos por rol. | React, Vite, Bootstrap, JS, CSS3 |
| [⚙️ **Panify-Backend**](https://github.com/Panify-HQ/Panify-Backend) | API RESTful encargada de la lógica de negocio, validaciones y reglas de inventario y pedidos. | Por definir |
| [📄 **Panify-Documentacion**](https://github.com/Panify-HQ/Panify-Documentacion) | Especificación técnica, Requisitos Funcionales (RF-001 a RF-004.6), modelo E-R y artefactos del SENA. | Markdown, Diagramas M.E.R. |

---

## 🚀 Módulos del sistema

| # | Módulo | Descripción |
| :-: | :--- | :--- |
| 1 | 🔑 **Autenticación y Control de Acceso** | Inicio de sesión con permisos por roles: `Cliente`, `Panadero`, `Domiciliario`, `Administrador` y `Super Administrador`. |
| 2 | 👤 **Gestión de Usuarios** | Registro de clientes, recuperación de contraseña y administración de perfiles con direcciones y barrios de entrega. |
| 3 | 🍞 **Productos e Inventario** | Control de existencias, cálculo de *Stock Mínimo*, alertas visuales de productos reponibles/agotados y actualización automática tras la compra. |
| 4 | 🛒 **Gestión de Pedidos** | Recepción de órdenes con validación de horario límite (bloqueo automático a las 6:00 PM) y congelamiento de precios al momento de la compra. |
| 5 | 🧾 **Gestión de Recibos** | Comprobantes en PDF por pedido y reportes operativos consolidados (diarios, semanales de lunes a domingo y mensuales). |
| 6 | 🚴 **Entregas y Logística** | Panel interactivo de prioridades por hora y franja para coordinar despachos en bicicleta con el domiciliario. |

---

## 🛠️ Stack tecnológico global

| Capa | Tecnologías |
| :--- | :--- |
| 🖥️ **Frontend** | React, Vite, Bootstrap, HTML5 semántico y CSS3 |
| ⚙️ **Backend** | API RESTful (tecnología por definir) |
| 🗄️ **Base de datos** | MySQL Workbench, modelo relacional normalizado en 3FN con jerarquía ISA |
| 🧪 **Simulación** | JSON Server para pruebas de integración |

---

## 👥 Equipo de desarrollo

| Integrante | Módulo / Responsabilidad |
| :--- | :--- |
| **Brayan Sneyder Devia Muñoz** | 🛒 Pedidos |
| **Brandon Duvan Guevara Rodríguez** | 🧾 Recibos |
| **Kevin Julián González Chavez** | 🔑 Autenticación y Usuarios |
| **Jeison Alejandro Diaz Acosta** | 🚴 Entregas |
| **Martin Cruz Muñoz** | 🍞 Productos |

---

## 🌿 Estándares y convenciones

### 🔀 Estrategia de ramificación
Uso de *Feature Branches* a partir de la rama de desarrollo:

- `feature/auth-login`
- `feature/gestion-usuarios`
- `feature/gestion-productos`
- `feature/gestion-pedidos`
- `feature/gestion-recibos`
- `feature/gestion-entregas`

### ✍️ Commits semánticos
Aplicación estricta de **Conventional Commits** para mantener un historial limpio y trazable:

`feat` · `fix` · `style` · `docs` · `refactor` · `chore`

---

<div align="center">

**Hecho por el equipo Panify · SENA ADSO**

</div>