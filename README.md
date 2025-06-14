# Proyecto Django CRUD de Estudiantes

Este es un proyecto web en Django que permite crear, leer, actualizar y eliminar registros de estudiantes.

## Requisitos

- Python 3.8 o superior
- pip
- Git
- Entorno virtual (opcional pero recomendado)

## Instalación

### 1. Clona el repositorio

```bash
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
```

### 2. Crea y activa un entorno virtual

#### En Windows:

```bash
python -m venv env
env\Scripts\activate
```

#### En macOS/Linux:

```bash
python3 -m venv env
source env/bin/activate
```

### 3. Instala las dependencias

```bash
pip install -r requirements.txt
```

> Si `requirements.txt` no existe, puedes crearlo con:
>
> ```bash
> pip freeze > requirements.txt
> ```

### 4. Configura la base de datos

```bash
python manage.py migrate
```

### 5. Crea un superusuario (opcional)

```bash
python manage.py createsuperuser
```

### 6. Ejecuta el servidor de desarrollo

```bash
python manage.py runserver
```

Visita [http://127.0.0.1:8000](http://127.0.0.1:8000) en tu navegador para ver la aplicación.

## Dependencias adicionales

Este proyecto utiliza:

- `django-widget-tweaks` para personalizar formularios en las plantillas.

### Para instalarlo:

```bash
pip install django-widget-tweaks
```

Y agrégalo en `settings.py`:

```python
INSTALLED_APPS = [
    ...
    'widget_tweaks',
]
```

## Estructura del proyecto

```
crud_project/
│
├── crud_project/       # Configuración principal del proyecto
├── estudiantes/        # Aplicación principal
├── templates/          # Plantillas HTML
├── static/             # Archivos estáticos (CSS, JS)
├── manage.py
└── README.md
```

## Licencia

Este proyecto está bajo la licencia MIT. Puedes usarlo y modificarlo libremente.
