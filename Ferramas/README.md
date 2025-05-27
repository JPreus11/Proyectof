
# Ferramas - Sistema de Gestión para Ferretería

Ferramas es un prototipo de sistema web para una ferretería, desarrollado en Python con Django como framework principal. El proyecto busca centralizar la administración de productos, usuarios y ventas, integrando un diseño funcional y operaciones CRUD básicas.

## 🧩 Tecnologías y Recursos Utilizados

- **Python 3.13**
- **Django 5.x**
- **SQLite3** como base de datos
- **Bootstrap 5** para el diseño visual
- **HTML5 / CSS3 / JS**
- **Iconos**: Bootstrap Icons
- **Sistema operativo de desarrollo**: Windows 11
- **Editor**: Visual Studio Code

## 🛠️ Requisitos para Ejecutar el Proyecto

### 1. Clona el repositorio
```bash
git clone https://github.com/JPreus11/ferramas
cd ferramas
```

### 2. Crea y activa un entorno virtual (recomendado)
```bash
python -m venv env
env\Scripts\activate     # En Windows
# source env/bin/activate  # En Linux/Mac
```

### 3. Instala las dependencias necesarias
```bash
pip install -r requirements.txt
```

> Si no tienes `requirements.txt`, instala manualmente:
```bash
pip install django
```

### 4. Aplica las migraciones y crea la base de datos
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Ejecuta el servidor local
```bash
python manage.py runserver
```

Luego, accede en tu navegador a:
```
http://127.0.0.1:8000/
```

### 6. Crear un superusuario para acceder al panel de administración
```bash
python manage.py createsuperuser
```

## 📁 Estructura del Proyecto

```
ferramas/
├── manage.py
├── ZonaGamers/               # Aplicación principal
│   ├── models.py             # Modelos (Juego, Cliente, etc.)
│   ├── views.py              # Lógica de las vistas
│   ├── urls.py               # Enrutamiento interno
│   ├── templates/
│   └── static/
├── Django_Ecommerce/         # Configuración general del proyecto
│   ├── settings.py
│   └── urls.py
└── db.sqlite3                # Base de datos local
```

## ✅ Funcionalidades Actuales

- Gestión CRUD de productos
- Registro de clientes
- Carrito de compras
- Interfaz limpia con Bootstrap
- Panel de administración de Django

## 📌 Notas importantes

- El directorio `static/` debe crearse si no existe.
- Verifica que el campo `codigo` en el modelo `Juego` sea único.
- En caso de errores de migración por claves duplicadas, borra la base de datos y vuelve a migrar (`db.sqlite3`).

## 📝 Licencia

Este proyecto es un prototipo académico sin fines comerciales.

---

Desarrollado por: 
Juan Farías
Camilo Ossandon
Iris Jara