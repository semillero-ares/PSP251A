# README

Para poder usar está plantilla para la documentación del proyecto deberemos preparar nuestro entorno de trabajo. Vamos a realizar la siguientes instalaciones:

- [Python](https://www.python.org/downloads/). Es importante activar la opción en el instalador `Add Python.exe to PATH`. 
- [Visual Studio Code](https://code.visualstudio.com/download).

En visual studio code, presionamos `Ctrl + J` para abrir el terminal, instalamos virtualenv con el siguiente comando:

```bash
pip install virtualenv
```

Creamos un ambiente virtual, en el ejemplo lo cree en la ruta `C:\virtualenv\mkdocs``, pero pueden usar cualquier ruta. 

```bash
python -m virtualenv C:\virtualenv\mkdocs
```

Y activamos luego, el ambiente virtual (el ejemplo es para windows):

```bash
C:\virtualenv\mkdocs\Scripts\Activate.ps1  
```

Si hay un error entonces, abrir un PowerShell en modo administrador y poner el siguiente comando:

```sh
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser
```

Abrimos la carpeta donde crearas la documentación (`Ctrl + K` seguido de `Ctrl + O`). 

Y estando allí, en el terminal: Activamos el ambiente virtual  e instalamos los requerimientos. 

```bash
C:\virtualenv\mkdocs\Scripts\Activate.ps1  
pip install -r .\requirements.txt
```

# Activan el servidor

```sh
C:\virtualenv\mkdocs\Scripts\Activate.ps1  
mkdocs serve
```