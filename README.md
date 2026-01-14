# 🔬 High-Energy Data Analysis with PyROOT: Caso Comercio Internacional

Este repositorio contiene un análisis técnico especializado utilizando el framework **ROOT** (CERN) a través de su interfaz de Python, **PyROOT**. El proyecto demuestra la capacidad de procesar formatos de datos binarios masivos (`.root`) y realizar ajustes estadísticos complejos, aplicando herramientas estándar de la física de partículas al análisis de flujos comerciales internacionales.

## 📝 Descripción del Problema
En el análisis económico, el manejo de grandes volúmenes de datos transaccionales requiere herramientas altamente eficientes. Este proyecto aborda el reto de procesar bases de datos de **exportaciones globales**, donde la memoria y la precisión estadística son críticas. Se busca identificar tendencias, calcular agregados masivos y modelar el comportamiento comercial entre naciones utilizando una infraestructura de alto rendimiento.

## 🎯 Objetivos del Proyecto
* **Procesamiento Eficiente:** Manejo de estructuras de datos `TTree` y `TBranch` para el acceso rápido y optimizado a grandes volúmenes de eventos comerciales.
* **Modelado Estadístico:** Implementación de ajustes de funciones (**Curve Fitting**) y **Regresión Lineal** para la extracción de tendencias de crecimiento y caracterización de flujos.
* **Visualización Científica:** Generación de gráficos de alta calidad (histogramas y gráficas de dispersión) con leyendas técnicas y cajas de estadísticas detalladas.

## 🛠️ Tecnologías y Herramientas
* **Lenguajes:** Python, C++ (Back-end de ROOT).
* **Librerías Principales:** PyROOT, NumPy, Pandas, Scikit-learn (para validación cruzada).
* **Gestión de Entorno:** Conda (Conda-Forge).

## 📊 Componentes del Análisis

### 1. Exploración y Procesamiento de Datos
* **Inspección de Jerarquías:** Análisis de archivos `.root` para identificar variables críticas como volúmenes de exportación, socios comerciales y periodos.
* **Cálculo de Totales:** Uso de iteradores eficientes en PyROOT para calcular el valor total de exportaciones por país de reporte.

### 2. Generación de Histogramas
* **Distribución de Frecuencias:** Creación de objetos `TH1F` para analizar la densidad de las transacciones y detectar picos o anomalías en el comercio internacional.

### 3. Modelado: Regresión y Ajuste (Fitting)
* **Ajuste de Funciones:** Aplicación de modelos lineales para cuantificar la tasa de crecimiento comercial.
* **Extracción de Parámetros:** Validación del modelo mediante la interpretación de los coeficientes de ajuste obtenidos directamente desde el motor de ROOT.

## 🚀 Instalación y Reproducibilidad

Para asegurar que el entorno sea reproducible y evitar conflictos de dependencias de C++, se recomienda el uso de **Conda**:

```bash
# Crear el entorno con ROOT pre-instalado
conda create --name root_env -c conda-forge root

# Activar el entorno
conda activate root_env

# Instalar soporte para Jupyter si es necesario
conda install ipykernel
python -m ipykernel install --user --name root_env --display-name "Python 3 (PyROOT)"

# Abrir el notebook
jupyter notebook
