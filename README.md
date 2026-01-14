# 🔬 High-Energy Data Analysis with PyROOT

Este repositorio contiene un análisis técnico especializado utilizando el framework **ROOT** (CERN) a través de su interfaz de Python, **PyROOT**. El proyecto demuestra la capacidad de procesar formatos de datos binarios masivos (`.root`) y realizar ajustes estadísticos complejos, herramientas estándar en la física de partículas y la investigación científica de alto nivel.

## 🎯 Objetivos del Proyecto
* **Procesamiento Eficiente:** Manejo de estructuras de datos `TTree` y `TBranch` para el acceso rápido a grandes volúmenes de eventos.
* **Modelado Estadístico:** Implementación de ajustes de funciones (Curve Fitting) para la extracción de parámetros físicos y caracterización de señales.
* **Visualización Científica:** Generación de gráficos con calidad de publicación, incluyendo leyendas técnicas y cajas de estadísticas detalladas.

## 🛠️ Tecnologías y Herramientas
* **Lenguajes:** Python, C++ (Back-end de ROOT).
* **Librerías Principales:** PyROOT, NumPy.
* **Gestión de Entorno:** Conda (Conda-Forge).

## 📊 Componentes del Análisis
1. **Exploración de Datos:** Inspección de la jerarquía de archivos `.root` para identificar variables críticas.
2. **Generación de Histogramas:** Creación de distribuciones de frecuencia (`TH1F`) para análisis de variables como energía, momento o masa invariante.
3. **Ajuste de Funciones (Fitting):** Aplicación de modelos Gaussianos y polinomiales para la separación de señal y ruido de fondo.

## 🚀 Instalación y Reproducibilidad

Para asegurar que el entorno sea reproducible y evitar conflictos de dependencias de C++, se recomienda el uso de **Conda**:

```bash
# Crear el entorno con ROOT pre-instalado
conda create --name root_env -c conda-forge root

# Activar el entorno
conda activate root_env

# Abrir el notebook
jupyter notebook
