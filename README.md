# Proyecto Django

Proyecto base para desarrollar con Django y Python.

## Requisitos

- Python 3.12
- Git

## Crear y activar el entorno virtual

En Windows PowerShell:

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Si PowerShell bloquea la activacion, ejecuta una vez:

```powershell
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

En macOS o Linux:

```bash
python3.12 -m venv .venv
source .venv/bin/activate
```

## Instalar Django

Con el entorno virtual activo:

```powershell
python -m pip install --upgrade pip
python -m pip install django
```

Para instalar todas las dependencias guardadas del proyecto:

```powershell
python -m pip install -r requirements.txt
```

Para guardar las dependencias del proyecto:

```powershell
python -m pip freeze > requirements.txt
```

## Iniciar el proyecto

```powershell
django-admin startproject config .
python manage.py runserver
```

El servidor estará disponible en <http://127.0.0.1:8000/>.

## Desactivar el entorno virtual

```powershell
deactivate
```
