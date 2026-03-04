# EatUpPagos 💳

Bienvenido al repositorio central del **Módulo de Pagos** de la aplicación **EatUp**. 
Este proyecto se desarrolla bajo una arquitectura de **microservicios** como parte de la materia **Software 3** en la **Universidad Católica de Oriente (UCO)**.

---

## 📌 Información del Proyecto
* **Semestre:** 2026-1
* **Institución:** Universidad Católica de Oriente (Rionegro, Antioquia)
* **Materia:** Software 3
* **Docente:** NOREÑA BLANDÓN JUAN PABLO

---

## 🏗️ Arquitectura de Microservicios

El módulo de Pagos es responsable de la gestión financiera del sistema y se divide en los siguientes microservicios:

### Equipo de Desarrollo y Responsables

| Microservicio | Responsable | Foto (Click para ir al Perfil) |
| :--- | :--- | :---: |
| **FACTURAS** | *Tomas Hernando Gomez* | <a href="https://github.com/TomasCGH"><img src="https://avatars.githubusercontent.com/u/169168247?v=4" width="80" height="80" style="border-radius: 50%;"></a> |
| **RECIBOS DE CAJA** | *Jean Paul Ortiz Restrepo* | <a href="https://github.com/jeanortiz22"><img src="https://avatars.githubusercontent.com/u/170052678?v=4" width="80" height="80" style="border-radius: 50%;"></a> |

---


## 📁 Estructura del Repositorio

Cada carpeta a nivel de raíz representa un microservicio independiente.

```bash
EatUpPagos/
├── FACTURAS/          # Gestión de facturación
└── RECIBOS_CAJA/      # Registro de pagos
```

## 🚀 FLUJO DE TRABAJO GITHUB - PROYECTO

```bash

# 1️⃣ Clonar repositorio
git clone <URL_DEL_REPOSITORIO>

# 2️⃣ Entrar al proyecto
cd EatUpPagos

# 3️⃣ Cambiar a rama de desarrollo
git checkout development

# 4️⃣ Crear rama para nueva funcionalidad
git checkout -b feature/nombre-funcionalidad

# Verificar rama actual
git branch

# ==========================================
# 🔎 ANTES DE SUBIR CAMBIOS
# ==========================================

# Ver si hay cambios nuevos en el repositorio remoto
git fetch

# Revisar historial de cambios
git log --oneline --graph --all

# Actualizar tu rama
git pull origin development

# ==========================================
# 📦 PREPARAR CAMBIOS
# ==========================================

git status
git add .
git commit -m "Descripción clara y detallada de la funcionalidad implementada"
git push -u origin feature/nombre-funcionalidad

# ==========================================
# 🔁 CREAR PULL REQUEST
# ==========================================

# Ir a GitHub
# Crear Pull Request hacia la rama development
# Agregar título claro y descripción detallada
# Esperar revisión antes de hacer Merge
# Eliminar la rama una vez fusionada

# ==========================================
# 🌳 ESTRUCTURA DE RAMAS
# ==========================================

# main         -> Producción (estable)
# development  -> Desarrollo
# feature/*    -> Ramas individuales

```

## 📁 📚 Documentación obligatoria por Microservicio

Para mantener orden, claridad y facilitar la integración entre equipos, **cada microservicio debe incluir dentro de su propia carpeta un archivo de documentación**.

Se recomienda crear dentro de cada carpeta de microservicio su propio README:

- `README.md` (preferido ✅)  
  ó  
- `estructura.txt`

---

### 📌 ¿Qué debe contener esta documentación?

Cada microservicio debe documentar obligatoriamente:

---

### 🗄 1️⃣ Esquema de Base de Datos

Debe incluir:

- Nombre de la tabla  
- Campos  
- Tipo de dato  
- Clave primaria (PK)  
- Claves foráneas (FK)  
- Relaciones

---

### 🔌 2️⃣ Endpoints que expone el microservicio

Debe documentarse cada endpoint con:

- Método HTTP (GET, POST, PUT, DELETE)  
- Ruta  
- Descripción  
- JSON de entrada (Request)  
- JSON de salida (Response)

---

## 🎯 Objetivos del Módulo Pagos

- Gestionar emisión de facturas 
- Registrar pagos totales o parciales
- Generar recibos de caja
- Integrarse correctamente con el módulo Comercial
- Mantener contratos API claros entre equipos

---

## 🚨 Regla del equipo

Ningún microservicio podrá integrarse a la rama development sin:
- La documentación completa
- Endpoints definidos
- Esquema de base de datos documentado
- Revisión aprobada
La documentación hace parte del entregable obligatorio.
