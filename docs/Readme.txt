# Instalar entorno virtual

    pip install virtualenv

# Crear entorno virtual

    virtualenv env

# Activar entorno virtual

    cd env 

    cd scripts

    activate 

    Si no funciona (PS E:\Escritorio\Damian\Programacion\fastapi-template\env\Scripts>)

            Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process

            .\activate

# Otra forma de activar entorno

    Crear entorno virtual: 
                        py -3 -m venv .venv

    Activar entorno: 
                    cd PATH\.venv\Scripts\Activate.ps1

# Instalar fastapi

    pip install fastapi  (framework)
    pip install uvicorn  (servidor)

# Instalar dependecias en VE:   
                                cd /ruta/a/tu/proyecto + pip install -r requirements.txt
                                ls

# Levantar App localmente: 
                            E:\Escritorio\Damian\Programacion\translate-fastapi\app> -> uvicorn main:app --reload

                            Quit -> CTRL + C

# Crear Proyecto

/my_project
│
├── /app
│   ├── /api
│   │   ├── /v1
│   │   │   ├── __init__.py
│   │   │   ├── endpoints.py
│   │   │   ├── models.py
│   │   │   ├── schemas.py
│   │   │   └── services.py
│   │   └── /v2 (opcional, para diferentes versiones de API)
│   │       ├── __init__.py
│   │       ├── endpoints.py
│   │       ├── models.py
│   │       ├── schemas.py
│   │       └── services.py
│   │
│   ├── /core
│   │   ├── config.py
│   │   └── security.py
│   │
│   ├── /db
│   │   ├── base.py
│   │   ├── session.py
│   │   └── migrations/
│   │
│   ├── /tests
│   │   ├── /unit
│   │   ├── /integration
│   │   └── conftest.py
│   │
│   ├── main.py
│   └── __init__.py
│
├── /docs
│   └── README.md
│
├── /scripts
│   └── setup.sh
│
├── /venv (si usas un entorno virtual)
├── requirements.txt
├── .env
└── .gitignore


