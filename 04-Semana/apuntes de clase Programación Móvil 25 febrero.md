# **Clase Programación Móvil**
📅 **Fecha:** 25/02/2025  

## **1. Actividades**
- 📌 Revisión y actualización de los tableros en Trello.  
- 📌 Resolución de dudas sobre la organización de las tareas.  

---

## **2. Conceptos Claves**

### **2.1. Análisis de Negocio en un Proyecto**
**📌 Semana 4 - Evaluación de Historias de Usuario**  

### **Resumen de la Semana**
- Se evaluaron las **Historias de Usuario (HU)** y su correcta redacción.  
- Se llevó a cabo un **ejercicio práctico**: diseño inicial de un mockup para una HU.  
- Introducción a la herramienta **Figma** para la creación de prototipos.  

### **Estructura de una Historia de Usuario**
1. **Descripción:** Rol del usuario y el objetivo que desea lograr.  
2. **Criterios de Aceptación:** Reglas que deben cumplirse para validar la HU.  
3. **Criterios de Finalización:** Condiciones necesarias para concluir la HU.  

#### **Ejemplo:**  

**Descripción:**  
> Como administrador del sistema, deseo gestionar las categorías de productos (crear, actualizar, eliminar y consultar) para garantizar una organización eficiente.  

**Criterios de Aceptación:**  
- Implementación de las funciones CRUD para las categorías.  
- Validaciones de campos requeridos.  

**Criterios de Finalización:**  
- Código funcional y testeado.  
- Revisión y aprobación del Product Owner.  
- Actualización de la documentación.  

### **Ejercicio Práctico**
- 🔹 Creación de un mockup para la HU del **Carrito de Compras**.  
- 🔹 Diseño inicial revisado en clase.  
- 🔹 Introducción básica a **Figma**.  
- 🔗 **Enlace del Mockup:** [Ver en Figma](https://www.figma.com/design/NIEpjfQmtZMCts9b4FzQAp/Untitled?node-id=0-1&t=nn1rIwqPMCYFKEzU-1)  

### **Planes para la Próxima Semana**
- 📌 Ampliar conocimientos en **Figma**.  
- 📌 Integrar los mockups en las historias de usuario dentro de **Trello**.  

---

## **3. Modelado y Diseño del Proyecto**

### **3.1. Componentes Básicos del Proyecto**
- **Base de datos** con sus tablas clave.  
- **Relaciones entre entidades** claras y definidas.  

#### **Ejemplo de Entidad Cliente:**
```json
{
    "cliente": {
        "nombre": "Ana",
        "apellido": "Gómez",
        "fecha_nacimiento": "1995-08-20",
        "correo": "anagomez@email.com"
    }
}
```

### **3.2. Buenas Prácticas**
- ✔ Análisis detallado de cada módulo.  
- ✔ Diseño organizado y claro.  
- ✔ Validación del comportamiento esperado de cada módulo.  

#### **Ejemplo de Módulos:**
- 📦 **Gestión de Inventario**  
- 🧾 **Facturación (POO)**  
- ⚙ **Configuración del Sistema**  
- 🛒 **Procesos de Venta**  
- 🔐 **Control de Acceso y Seguridad**  

---

## **4. Modelado de Datos**

📌 **Requisitos del Modelo de Datos:**  
- ✅ Enfoque **iterativo e incremental**.  
- ✅ Contar con un **diagrama de base de datos**.  
- ✅ Incorporar un **diagrama de secuencias**.  

---

## **5. Arquitectura del Proyecto**

📌 **Conceptos Fundamentales:**  
- Ejemplo de **arquitectura modular**: **Nequi**.  
- Posibilidad de reutilizar datos para diferentes roles (ej. cliente, administrador).  
- Inclusión de **procesos tercerizados** según las necesidades del sistema.  

---

## **6. Configuración del Sistema**

📌 **Inserción y control de datos en la base de datos**.  
📌 **Ejemplos de Parámetros:**  
- 🌐 **Selección de idioma**  
- 🕒 **Definición de horarios laborales**  
- 📅 **Gestión de eventos y reservas**  
- 📊 **Configuración de periodos de tiempo**  

---

## **7. Historias de Usuario (HU) y Buenas Prácticas en Scrum**

📌 **Ejemplo de Entidad Categoría:**
```json
{
    "Categoria": {
        "id": "auto_increment",
        "codigo": "único",
        "nombre": "requerido",
        "descripcion": "opcional",
        "estado": "activo por defecto"
    }
}
```

---

## **8. Diseño y Distribución de Tareas**

📌 **Tareas Divididas en Módulos:**
- 🎨 **Diseño UI/UX (mockup)**  
- 🔙 **Desarrollo Backend**  
- 🖥 **Implementación Frontend**  
- 🗄 **Creación y gestión de la base de datos**  
- ⚙ **Infraestructura y despliegue (DevOps)**  
- 📄 **Elaboración de documentación**  

---

## **9. Estimación y Entrega de HU**

📌 **Historia de Usuario:**

### **Descripción:**
> Como administrador del sistema, quiero poder gestionar las categorías de productos para asegurar su correcta organización y fácil acceso.  

### **✅ Criterios de Aceptación:**

🔹 **Agregar Categorías:**
- Registrar una nueva categoría con los siguientes campos:  
  - `id` (autogenerado)  
  - `codigo` (único)  
  - `nombre` (obligatorio)  
  - `descripcion` (opcional)  
  - `estado` (activo/inactivo)  

🔹 **Modificar Categorías:**
- Actualizar `nombre`, `descripcion` y `estado`.  
- ❌ No modificar `id` ni `codigo` una vez creados.  

🔹 **Eliminar Categorías:**
- ❌ Solo si no están vinculadas a productos.  

🔹 **Consultar Categorías:**
- Visualizar todas las categorías registradas.  
- Filtrar por `codigo` y `nombre`.  

### **✅ Criterios de Finalización:**
✅ Funcionalidad completada y testeada.  
✅ Aprobación en revisión de código (Pull Request).  
✅ Demostración al **Product Owner**.  
✅ Documentación actualizada.  

