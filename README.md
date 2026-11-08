# synthetic-audio-detection

Proyecto de detección de audios naturales y sintéticos mediante la fusión de predicciones de cuatro modelos DenseNet121 con Machine Learning.

## Contenido del repositorio

| Archivo o carpeta | Descripción |
|---|---|
| `Deteccion_Audios_Sinteticos.ipynb` | Notebook con el desarrollo del proyecto. |
| `Documentacion_Tecnica.md` | Justificación técnica del método y análisis de resultados. |
| `data/` | Datos utilizados en el proyecto. |
| `requirements.txt` | Dependencias de Python. |
| `.gitignore` | Archivos y carpetas excluidos del control de versiones. |

## Requisitos

- Python 3.13. La configuración inicial se realizó con Python 3.13.14.
- Visual Studio Code con las extensiones **Python** y **Jupyter** de Microsoft.
- Git, para clonar el repositorio y colaborar.

## Configuración del entorno

Después de clonar el repositorio, cada integrante deberá abrir la carpeta del proyecto en VS Code y ejecutar los siguientes comandos en la terminal de PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

El primer comando crea el entorno virtual `.venv`. El segundo instala las dependencias del proyecto dentro de ese entorno.

Cada integrante deberá crear su propio entorno en su computador. La carpeta `.venv` está excluida de Git y no se sube al repositorio.

Esta configuración se realiza una sola vez por copia local del proyecto.

## Ejecución del notebook

Para ejecutar el proyecto, se deberá:

1. Abrir `Deteccion_Audios_Sinteticos.ipynb` en VS Code.
2. Pulsar el selector de kernel ubicado en la esquina superior derecha del notebook.
3. Seleccionar **Python Environments → .venv**. Si ya hay otro kernel seleccionado, acceder primero a **Select Another Kernel**.
4. Comprobar que la ruta del intérprete termine en `.venv\Scripts\python.exe`.
5. Ejecutar las celdas en orden, desde el inicio.

El kernel seleccionado permite ejecutar el notebook con el Python y las dependencias instaladas en el entorno del proyecto.

## Si no aparece el selector de kernel

Cuando ya existe un kernel seleccionado, el botón puede mostrar su nombre, por ejemplo, **Python 3.13.14**, en lugar de **Select Kernel**.

Si el notebook se abre como texto, se deberá hacer clic derecho sobre el archivo y seleccionar **Open With… → Jupyter Notebook**.

Si esa opción no está disponible, se deberá comprobar que las extensiones **Python** y **Jupyter** de Microsoft estén instaladas y habilitadas.

## Actualización de dependencias

Cuando se incorporen nuevas librerías al proyecto, se deberá actualizar `requirements.txt`.

Después de descargar esos cambios, cada integrante deberá ejecutar:

```powershell
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

No será necesario crear nuevamente el entorno virtual.
