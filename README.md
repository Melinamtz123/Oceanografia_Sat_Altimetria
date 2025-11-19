#  TP9: Nivel del Mar y Circulación

##  Materia: Oceanografía Satelital / Teledetección Satelital y Aplicaciones Oceanográficas
**Cuatrimestre:** 2do Cuatrimestre 2025
**Unidad Temática:** Topografía superficial del mar. Circulación oceánica


---

##  Objetivo Principal del Trabajo Práctico

El objetivo de este trabajo práctico es que el alumno obtenga datos de la **Altura del Nivel del Mar** (SSH/SLA) y de las **Velocidades Geostróficas** asociadas, y los compare con la trayectoria real de una **boya derivante** (Drifter) a elección.

##  Contenido del Repositorio

| Archivo | Descripción |
| :--- | :--- |
| `TP09_altimetria_2025.pdf` | **Guía Principal** del Trabajo Práctico (PDF). Contiene el objetivo, la metodología y los pasos para el análisis. |
| `TP09_altimetria.ipynb` | **Script de Python** (Jupyter Notebook) para la visualización y análisis de los datos de altimetría y boyas. |
| `README.md` | Este documento. |
| **Material Ejercitación Adicional** | Ejercicios complementarios para profundizar en la unidad de altimetría. |

---

## 🛠️ Material Adicional de Ejercitación Práctica

Se presentan tres ejercicios adicionales diseñados para complementar el TP09 y reforzar las habilidades en el manejo y la selección de datos de altimetría y boyas derivantes.

### 1.  Ejercicio de Exploración y Selección de Boyas

* **Objetivo:** Profundizar en la identificación de boyas adecuadas para la validación de la altimetría.
* **Procedimiento:**
    1.  Acceder al visualizador del Global Drifter Program: `https://www.aoml.noaa.gov/phod/gdp/interactive/drifter_array.html`.
    2.  Seleccionar una boya que cumpla con los siguientes criterios:
        * Trayectoria que siga una estructura de la circulación oceánica definida (ej., una corriente fuerte o un remolino/eddy).
        * Periodo de actividad de al menos **9 meses**.
        * Que **no haya perdido su ancla de capa** (drogue) en ese lapso.
    3.  **Registrar/Responder:** IMEI, WMO, Región geográfica (lat/lon aproximada), Fechas de inicio/fin del periodo de 9 meses, y la estructura de la circulación oceánica que la boya parece seguir.

### 2.  Ejercicio de Restricción de Datos en ERDDAP

* **Objetivo:** Practicar la aplicación de filtros geográficos y temporales para la descarga de subconjuntos de datos.
* **Contexto:** Utilizar el **ID de WMO** y las **fechas/región** de la boya seleccionada en el Ejercicio 1.
* **Tarea de Verificación:** Acceder al *dataset* `drifter_6hour_qc` en ERDDAP y aplicar las restricciones para la boya seleccionada. Crear un *screenshot* del formulario con todas las restricciones aplicadas (WMO, tiempo, latitud, longitud).

### 3.  Ejercicio de Análisis de Variables Geostróficas

* **Objetivo:** Entender la selección de variables clave en los productos de altimetría para el análisis de corrientes geostróficas.
* **Contexto:** Revisar las variables disponibles en el *dataset* de altimetría del Copernicus Marine Service (ej., `cmems_obs-sl_glo_phy-ssh_my_allsat-14-duacs-0.25deg_P1D`).
* **Preguntas a Responder:**
    1.  ¿Cuál es la diferencia física entre la **"Sea surface height above geoid"** y la **"Sea surface height above sea level"**? ¿Cuál se usa para calcular la Anomalía del Nivel del Mar (SLA)?
    2.  Además de la velocidad geostrófica total, ¿qué otras dos componentes de velocidad son necesarias para definir la dirección de la corriente?
    3.  Si la boya tiene una deriva neta hacia el **Norte**, ¿qué componente de la velocidad geostrófica debería tener el valor positivo más alto?

---

##  Guía de Acceso (Para Alumnos)

Hay dos formas de obtener este material:

### Opción A: Descarga Directa (ZIP)

Es la forma más sencilla para descargar el material sin necesidad de usar la línea de comandos.

1.  Haga clic en el botón verde **`< > Code`** ubicado en la parte superior derecha de esta página del repositorio.
2.  Seleccione la opción **"Download ZIP"**.
3.  Descomprima el archivo ZIP en su computadora.

### Opción B: Clonar el Repositorio (Para recibir actualizaciones)

Si tiene Git instalado, puede clonar el repositorio y mantenerlo actualizado fácilmente.

1.  Abra su terminal o *Git Bash*.
2.  Ejecute el comando `git clone` seguido de la URL del repositorio (la cual puede copiar del botón verde `< > Code`):

    ```bash
    git clone [https://aws.amazon.com/es/what-is/repo/](https://aws.amazon.com/es/what-is/repo/)
    ```

3.  Para obtener futuras actualizaciones de los archivos (si el profesor añade o modifica algo), solo necesita navegar a la carpeta del repositorio en su terminal y ejecutar:

    ```bash
    git pull

    ```

