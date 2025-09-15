# Proyecto Final F1

# Proyecto de Análisis Exploratorio de Datos (EDA) – Fórmula 1

Este repositorio contiene un análisis exploratorio de datos (EDA) realizado con **Python** sobre resultados de Fórmula 1 desde 2020.  

El proyecto utiliza dos datasets principales:  
- **Dataset (df_dataset):** Registro de todas las vueltas de cada piloto en cada carrera.  
- **Lastlap (df_lastlap):** Derivado del dataset, contiene únicamente la última vuelta de cada piloto en cada carrera, lo que facilita análisis de posiciones finales, vueltas rápidas y puntos.

---

## Objetivos
- Realizar una **limpieza y transformación completa** de los datos en bruto.  
- Explorar estadísticas descriptivas de pilotos, constructores y circuitos.  
- Generar **visualizaciones claras y variadas** que muestren patrones relevantes: evolución de posiciones, distribución de tiempos, análisis por constructor, etc.  
- Comparar la información de ambos datasets (`dataset` vs `lastlap`) para validar coherencia y extraer conclusiones.  

---

## Estructura del repositorio
El proyecto está organizado en notebooks de Jupyter:

1. **Carga y preparación de datos**  
   - Lectura del Excel original.  
   - Conversión de tiempos (`LapTime`, `fastestLapTime`) a segundos.  
   - Limpieza de columnas innecesarias y valores atípicos.  
   - Exportación de los datasets limpios en formato Parquet.  

2. **EDA Dataset**  
   - Estadísticas descriptivas de vueltas, posiciones y tiempos.  
   - Distribución de posiciones de salida y resultados.  
   - Evolución de vueltas rápidas y tiempos por temporada.  
   - Análisis de abandonos vs finalizaciones.  

3. **EDA Lastlap**  
   - Distribución de posiciones finales y podios.  
   - Análisis de vueltas rápidas (FASTLAP).  
   - Comparación grid inicial vs posición final.  
   - Rendimiento de pilotos y constructores en últimas vueltas.  

4. **Comparativa Dataset vs Lastlap**  
   - Validación de coherencia (últimas vueltas derivadas).  
   - Relación entre vueltas rápidas y resultados finales.  
   - Constructores con mayor consistencia en rendimiento.  

5. **Conclusiones**  
   - Resumen de hallazgos principales, con cifras concretas.  
   - Validación de hipótesis (ej. ventaja de salir en primera fila, distribución de FASTLAP por constructor).  
   - Ideas para análisis predictivos futuros.  

---

## Herramientas utilizadas
- **Lenguaje:** Python  
- **Librerías principales:**  
- `pandas`, `numpy`, `matplotlib`, `seaborn`.

---

## Datos extraidos de

- Formula 1 World Championship (1950-2024) – Kaggle: https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020
- F1DB (Open Source Formula 1 Database): https://github.com/f1db/f1db/releases
- ErgastF1 dataset (Relational / Fel.cvut): https://relational.fel.cvut.cz/dataset/ErgastF1
- Ergast Developer API / f1db CSV tables: http://ergast.com/downloads/f1db_csv.zip

