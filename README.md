# 🌦️ Simulación de Estados Climáticos y Niveles de Humedad mediante un Modelo Oculto de Markov (HMM)

**Actividad Didáctica 2-M2**  
**Institución:** Institución Universitaria Digital de Antioquia (IUDigital)  
**Fecha de entrega:** 15 Noviembre 2026

---

## 👥 Integrantes del Grupo 07
- Carolina Velásquez Ávila
- Johnatan Darío Vélez Betancur
- Elisabeth Martínez Hernández

---

## 📌 Descripción del Proyecto
Este repositorio contiene la implementación, simulación y análisis de un **Modelo Oculto de Markov (HMM)** aplicado a la predicción de condiciones climáticas (Soleado, Nublado, Lluvioso) a partir de observaciones de humedad (Baja, Media, Alta). 

El trabajo compara **tres escenarios experimentales** para analizar la sensibilidad y reproducibilidad del modelo, cumpliendo con los estándares de rigor científico exigidos para un artículo tipo Q1.

---

## 📂 Estructura del Repositorio
- `HMM_clima.ipynb`: Notebook principal con la implementación completa, validación de matrices y simulación de los 3 escenarios (300 réplicas c/u).
- `resultados_simulacion_hmm.csv`: Secuencia de 30 días del escenario base (semilla 42).
- `resultados_escenarios_900_replicas.csv`: Datos crudos de los 3 escenarios (900 simulaciones en total).
- `resumen_estadistico_escenarios.csv`: Tabla resumen con Media, Desviación Estándar, Mínimo, Máximo e IC 95%.
- `grafica_estados.png`, `grafica_humedad.png`, `grafica_dias_por_estado.png`, `grafica_estacionaria.png`: Evidencias gráficas del escenario base.
- `grafica_comparacion_humedad_alta.png`, `grafica_comparacion_persistencia.png`: Gráficas comparativas de los 3 escenarios con intervalos de confianza.

---

## ⚙️ Requisitos y Entorno
- **Lenguaje:** Python 3.x
- **Librerías:** `numpy`, `pandas`, `matplotlib`
- **Entorno recomendado:** [Google Colab](https://colab.research.google.com/) (no requiere instalación local).

---

## 🚀 Instrucciones de Ejecución
1. Abre el archivo `HMM_clima.ipynb` en Google Colab.
2. En el menú superior, selecciona **Entorno de ejecución** > **Ejecutar todo** (o presiona `Ctrl + F9`).
3. El código validará las matrices, ejecutará las 900 réplicas y generará automáticamente las tablas resumen y las gráficas.

---

## 🔬 Escenarios Evaluados
1. **Base:** Parámetros originales del ejemplo académico.
2. **Mayor persistencia climática:** Matriz de transición ($A$) ajustada para aumentar la probabilidad de permanecer en el mismo estado.
3. **Humedad más asociada al clima:** Matriz de emisión ($B$) ajustada para fortalecer la relación entre el estado oculto y la observación de humedad.

---


## 📜 Integridad Académica
- ✅ Código original desarrollado por los integrantes del grupo.
- ✅ Parámetros hipotéticos basados en ejemplo académico del curso.
- ✅ Semillas aleatorias documentadas (10000 a 10299) para garantizar total reproducibilidad.

---
**© 2026 Grupo 07 - IUDigital**
