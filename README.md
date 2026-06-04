# PilatesApp

Sistema de gestión para estudios de pilates con backend Django REST + Frontend Next.js.

## Stack

| Capa | Tecnología |
|------|-----------|
| Backend | Django 5 + Django REST Framework |
| Frontend | Next.js |
| Base de datos | SQLite (dev) / PostgreSQL (prod) |
| Infraestructura | Docker, Railway |

## Módulos del backend

- **accesos** — Control de acceso y autenticación
- **clases** — Programación y gestión de clases
- **empresas** — Configuración multi-tenant
- **estudios** — Gestión de estudios de pilates
- **notificaciones** — Sistema de notificaciones
- **pagos** — Procesamiento de pagos
- **progresos** — Seguimiento de progreso de alumnos
- **referidos** — Programa de referidos
- **sedes** — Gestión de sedes
- **usuarios** — Perfiles y roles de usuario

## Desarrollo local

```bash
# Backend
cd backend_django
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

# Frontend
cd frontend_nextjs
npm install
npm run dev
```

## Despliegue

La aplicación está configurada para desplegarse en Railway mediante `railway.json` y `Dockerfile`.
