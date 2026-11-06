# Entorno virtual conda: `mlops`

## Crear el entorno (solo la primera vez)

```bash
# Crear el entorno con Python 3.11 (la versión de .python-version)
conda create -n mlops -c conda-forge python=3.11 pip -y

# Activarlo
conda activate mlops

# Instalar las dependencias desde requirements.txt
python -m pip install -r requirements.txt

# Registrar el entorno como kernel de Jupyter (para los notebooks)
python -m ipykernel install --user --name mlops --display-name "Python (mlops)"
```

## Activar el entorno

```bash
conda activate mlops
```

Luego, en VS Code o Jupyter, elige el kernel **Python (mlops)** para los notebooks.

## Desactivar el entorno

```bash
conda deactivate
```

## Otros comandos útiles

```bash
# Ver los entornos disponibles
conda env list

# Borrar el entorno
conda env remove -n mlops
```
