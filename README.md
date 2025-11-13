# Introducción a Python (DAM)

Repo con notebooks para introducir en la programación con lenguaje Python.

## Estructura

- `notebooks/`: cuadernos Jupyter.
- `data/`: ficheros de datos usados por los notebooks.
- `env/requirements.txt`: dependencias de Python.

## Cómo usar este repositorio 

1. Haz **Fork** de este repositorio en tu cuenta de GitHub.
2. En tu máquina:
```bash
git clone https://github.com/TU-USUARIO/introduccion-python.git
cd python-dam-intro
```
3.	Crea un entorno (opcional pero recomendado):
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
# .venv\Scripts\activate   # Windows PowerShell
pip install -r env/requirements.txt
```
4.	Abre JupyterLab en la carpeta del repo:
```bash
jupyter lab
```


## 3. Cómo se debe trabajar en JupyterLab

Cuando ya tenemos el repositorio clonado:

1. Abrir **JupyterLab** desde la carpeta raíz del repo (`introduccion-python/`).
2. Navegar en el navegador de archivos de Jupyter hasta `notebooks/`.
3. Abrir, por ejemplo, `03_EstructurasDatos.ipynb`.
4. Si el notebook usa ficheros, las rutas deberían ser relativas, por ejemplo:

   ```python
   from pathlib import Path

   ROOT = Path("..")        # desde notebooks/ volvemos a la raíz
   DATA = ROOT / "data"

   csv_path = DATA / "alumnos.csv"  