<div align="center">

# Panify

### *Horneamos Calidad, Entregamos Confianza y Unimos Lazos.*

Aplicación web para la gestión de **pedidos, inventario y recibos** de la fabrica de pan **Distribuciones Oro Pan**.

![SENA](https://img.shields.io/badge/SENA-ADSO-39A900?style=for-the-badge)
![Ficha](https://img.shields.io/badge/Ficha-3315796-orange?style=for-the-badge)
![Grupo](https://img.shields.io/badge/Grupo-4-blue?style=for-the-badge)

</div>

---

## 📌 Sobre el proyecto

**Panify** nace de un caso real: la fabrica de pan *Distribuciones Oro Pan* registraba sus pedidos de forma manual (llamadas y papel), lo que generaba pérdida de información, retrasos en producción, confusiones para el domiciliario y falta de comprobantes claros para los clientes.

Panify centraliza y digitaliza ese flujo operativo para eliminar el registro manual, optimizar los tiempos de producción y entrega, y garantizar la trazabilidad de los productos.

> **Pregunta del proyecto:** ¿Cómo mejorar la recepción, organización y gestión de pedidos e inventario en Oro Pan?

> ⚠️ **Alcance:** sistema netamente operativo (pedidos y stock). No abarca procesos contables ni financieros externos.

---

## 🗂️ Repositorios

| Repositorio | Descripción |
|---|---|
| [**Panify-Documentacion**](https://github.com/Panify-HQ/Panify-Documentacion) | Requisitos (RF/RNF), modelo entidad-relación, scripts SQL, diagramas e investigación del proyecto. |
| [**Panify-Frontend**](https://github.com/Panify-HQ/Panify-Frontend) | Interfaz web (React + Vite, HTML5 semántico y CSS responsivo). |
| [**Panify-Backend**](https://github.com/Panify-HQ/Panify-Backend) | API y lógica de negocio, conectada a la base de datos MySQL. |

---

## 📦 Módulos del sistema

1. **🔐 Autenticación:** Registro de nuevos usuarios, inicio de sesión seguro, recuperación de contraseña y gestión de tokens y sesiones.
2. **👤 Gestión de Usuarios:** Administración de perfiles, historial de actividad/compras y control de acceso por roles (Administrador, Panadero, Domiciliario y Cliente).
3. **🍞 Gestión de Productos:** CRUD completo del catálogo de productos, control de stock mínimo, alertas de producto agotado y actualización automática del inventario al confirmar pedidos.
4. **🛒 Gestión de Pedidos:** Creación y seguimiento de órdenes validadas contra el stock disponible, con control horario (bloqueo de pedidos del mismo día después de la hora límite).
5. **🧾 Gestión de Recibos y Reportes:** Emisión de comprobantes en PDF por cada pedido y generación de reportes operativos (diarios, semanales y mensuales).
6. **🚴 Gestión de Entrega:** Panel de prioridades ordenado por hora y urgencia para el panadero y el domiciliario, junto con una lista de rutas optimizadas para entregas.

---

## 🗄️ Modelo de datos

Base de datos en **MySQL**, normalizada hasta **3FN**, con jerarquía de especialización (ISA) para el control de acceso:

- **Usuario** (entidad padre) → **Cliente**, **Domiciliario** y **Panadero** como subtipos.
- Entidades transaccionales: **Dirección**, **Producto**, **Pedido**, **Detalle_Pedido** y **Recibo**.
- Atributos derivados (`Total_Pagar`, `Subtotal`, `Estado_Stock`) calculados por código/SQL.

El detalle completo se encuentra en [Panify-Documentacion](https://github.com/ORGANIZACION/Panify-Documentacion).

---

## 🚀 Flujo de trabajo en Git

**Feature Branches** por módulo:

```
feature/auth-login
feature/gestion-usuarios
feature/gestion-productos
feature/gestion-pedidos
feature/gestion-recibos
feature/gestion-entregas
```

**Commits semánticos** (Conventional Commits):

```
<tipo>(<ámbito>): <descripción en imperativo y minúsculas, máx. 50 caracteres>
```

| Tipo | Uso |
|---|---|
| `feat` | Nueva funcionalidad |
| `docs` | Documentación |
| `style` | Estilos / formato |
| `refactor` | Reestructuración de código |
| `chore` | Tareas de mantenimiento |

Ámbitos comunes: `(ui)`, `(db)`, `(repo)`, `(trimestre3)`, `(cliente)`, `(admin)`.

Ejemplo: `feat(ui): agregar menú hamburguesa en landing`

---

## 🎓 Contexto académico

Proyecto formativo del **SENA – Análisis y Desarrollo de Software (ADSO)**, Ficha **3315796**, Grupo 4, desarrollado a lo largo de 7 trimestres de la etapa lectiva.

---

<div align="center">

**Panify** · Hecho para *Distribuciones Oro Pan*

</div>