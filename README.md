# 📊 Challenge de Análisis de Datos - Alura LATAM

## ✨ Descripción del Proyecto

Este proyecto presenta el análisis de datos realizado como parte del **Challenge de Data Science de Alura LATAM**. El objetivo fue explorar conjuntos de datos de ventas de varias tiendas para descubrir patrones, calcular métricas clave de negocio y obtener insights que puedan impulsar decisiones estratégicas. El análisis se documenta paso a paso en un Jupyter Notebook, listo para ser ejecutado en Visual Studio Code.

## 🚀 Configuración y Ejecución en VS Code

Sigue estos pasos para configurar el entorno y ejecutar el análisis utilizando Visual Studio Code.

### 📋 Prerrequisitos

Antes de comenzar, asegúrate de tener instalados:

- ✅ **Git**: Para clonar el repositorio.
- ✅ **Python 3.12**: La versión de Python que utilizarás.
- ✅ **Visual Studio Code**: El editor de código.
- ✅ **Extensión de Python para VS Code**: Busca "Python" por Microsoft en la vista de Extensiones de VS Code e instálala. Esencial para trabajar con Python y notebooks en VS Code.

### 🛠️ Herramienta Adicional Recomendada

> [!TIP]
> Para una experiencia más rica en la exploración de datos dentro de VS Code, ¡te sugiero encarecidamente instalar la extensión **Data Wrangler**!
>
> Esta extensión, también de Microsoft, es fantástica para:
>
> - Visualizar e inspeccionar DataFrames de pandas y otras variables de Python directamente mientras ejecutas tu código o el notebook.
> - Ver estadísticas resumen, filtrar datos y previsualizar transformaciones sin salir del editor.
>
> Simplemente búscala como **"Data Wrangler"** en la vista de Extensiones de VS Code e instálala. ¡Será tu mejor aliada para entender los datos a medida que avanzas en el notebook!

### 👇 Pasos para Ponerlo en Marcha

1.  **Clonar el repositorio:**

    Abre tu terminal o línea de comandos y descarga el código del proyecto:

    ```bash
    git clone https://github.com/RonyTrespalacios/challenge1-data-science-latam.git
    ```

    ```bash
    cd challenge1-data-science-latam
    ```

2.  **Crear un Entorno Virtual:**

    Creamos un entorno aislado para las dependencias del proyecto.

    ```bash
    python -m venv .venv
    ```

    Esto creará una carpeta `.venv` dentro de tu proyecto con una instalación limpia de Python.

3.  **Activar el Entorno Virtual:**

    Ahora, activa el entorno virtual que acabas de crear.

    - En **Windows Command Prompt** o **PowerShell**:

      ```bash
      Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
      ```

      ```bash
      .\.venv\Scripts\activate
      ```

    - En **Git Bash**, **WSL**, **macOS** o **Linux**:
      ```bash
      source .venv/bin/activate
      ```

> [!TIP]
> Sabrás que el entorno está activo porque verás `(.venv)` al principio de tu prompt en la terminal.

4.  **Instalar las Dependencias:**

    Las dependencias del proyecto se gestionan usando `requirements.txt`. Con el entorno virtual **activo**, instala todas las librerías necesarias:

    ```bash
    pip install -r requirements.txt
    ```

> [!NOTE]
> Este comando lee el archivo `requirements.txt` e instala todas las librerías listadas en él.

5.  **Abrir el Proyecto en VS Code:**

    Si no lo tienes abierto, inicia VS Code y abre la carpeta del proyecto que acabas de clonar (`challenge1-data-science-latam`).

    ```bash
    code .
    ```

> [!TIP]
> Si ya estás en la terminal dentro de la carpeta del proyecto y VS Code está agregado a tu PATH, puedes simplemente ejecutar `code .` para abrir el proyecto rápidamente.

6.  **Seleccionar el Intérprete de Python del Entorno Virtual:**

    Este es un paso **fundamental** para asegurarte de que VS Code use las librerías que instalaste _dentro de tu entorno virtual_.

    - Abre la Paleta de Comandos de VS Code: Presiona `Ctrl+Shift+P` (Windows/Linux) o `Cmd+Shift+P` (macOS).
    - Escribe `Python: Select Interpreter` y selecciona esa opción.
    - VS Code buscará intérpretes en tu proyecto. Busca y selecciona el intérprete que se encuentra dentro de la carpeta `.venv`. Generalmente se verá algo como `./.venv/bin/python` o `.\.venv\Scripts\python.exe`, posiblemente con el nombre `(.venv)` o `Python (...) .venv`.

> [!IMPORTANT]
> Si no seleccionas el intérprete correcto, VS Code podría intentar usar la instalación global de Python y no encontrará las librerías del proyecto, lo que causará errores al ejecutar el notebook.

7.  **Abrir y Ejecutar el Notebook:**

    - En el explorador de archivos de VS Code, navega hasta el archivo `AluraStoreLatam.ipynb` y haz clic para abrirlo.
    - VS Code abrirá el notebook en su editor integrado.
    - Verifica en la esquina superior derecha del notebook que el kernel seleccionado sea el de tu entorno virtual (debería decir algo como `Python 3.12 (.venv)`). Si no es así, haz clic en él para cambiarlo.
    - Ahora puedes ejecutar cada celda de código individualmente haciendo clic en el ícono ▶️ a la izquierda de la celda, o usar los controles en la parte superior del notebook para ejecutar todas las celdas.

> [!NOTE]
> El archivo `.ipynb` contiene tanto el código como los resultados. Puedes limpiar los resultados si quieres antes de ejecutarlo, o simplemente ejecutar las celdas secuencialmente.

8.  **Desactivar el Entorno Virtual:**

    Cuando hayas terminado de trabajar en el proyecto y cierres VS Code, es una buena práctica desactivar el entorno virtual. Regresa a la terminal donde lo activaste y ejecuta:

    ```bash
    deactivate
    ```

¡Eso es todo! Ya tienes el proyecto configurado y listo para ser explorado y ejecutado en VS Code.

---

## 🧐 Análisis Destacado

Este proyecto explora:

- Importación y caracterización inicial de los datos.
- Análisis de la facturación total por tienda.
- Identificación de las categorías de productos con más ventas.
- Cálculo de la calificación promedio por tienda.
- Análisis de los productos más y menos vendidos.
- Determinación del costo promedio de envío.
- Visualizaciones clave para entender los insights.

---

## 🎯 Conclusiones Principales

Basado en el análisis, algunas conclusiones relevantes incluyen:

- La tienda con menor facturación identificada es la **Tienda 4**.
- La **Tienda 4** también se encuentra entre las tiendas con mayor tasa de calificaciones bajas (menores a 3 estrellas).

Estos insights sugieren áreas potenciales de mejora o investigación adicional para la Tienda 4.

---

## 🧑‍💻 Autor

- [Rony Trespalacios](https://github.com/RonyTrespalacios)

---

## 🙏 Agradecimientos

- A Alura LATAM por proponer este interesante challenge de análisis de datos.
- A la comunidad de Python por las increíbles librerías.

---
