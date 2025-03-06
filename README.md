# 🏦 Análisis de Fraude con Tarjetas de Crédito

Este proyecto tiene como objetivo identificar patrones comunes en transacciones fraudulentas utilizando **Python, SQL (BigQuery) y técnicas de análisis de datos**.

---

## 📊 Objetivo del Proyecto

El análisis busca detectar **patrones en transacciones fraudulentas** para comprender mejor los factores asociados a fraudes con tarjetas de crédito. Esto puede ayudar en la detección temprana y prevención de fraudes.

---

## 🔍 Dataset

- **Fuente:** Dataset sintético de transacciones con tarjetas de crédito.  
- **Principales columnas:**
  - `Transaction_ID` → Identificador único de la transacción.
  - `Transaction_Amount` → Monto de la transacción.
  - `Timestamp` → Fecha y hora de la transacción.
  - `Location` → Ciudad donde ocurrió la transacción.
  - `Transaction_Type` → Tipo de transacción (compra, retiro, transferencia, etc.).
  - `Is_Fraudulent` → 1 si es fraude, 0 si es legítima.
  - `Deviation_From_Avg` → Desviación respecto al monto promedio del usuario.

---

## 🛠️ Tecnologías Usadas

- **Python** 🐍 (Pandas, Matplotlib, Seaborn)
- **SQL (Google BigQuery)** 📊
- **Google Colab** (para análisis interactivo)
- **GitHub** (documentación y versionado de código)

---

## 📈 Análisis Realizado

### 1️⃣ **Exploración de Datos**
- Revisión de valores nulos y duplicados.
- Distribución de montos en transacciones fraudulentas vs. legítimas.
- Análisis de la desviación estándar en montos de transacción.

### 2️⃣ **Identificación de Patrones en Fraudes**
- **¿Qué tipos de transacción tienen más fraude?**  
  🔹 Transferencias y retiros tienen una tasa de fraude más alta que compras.  
- **¿En qué rango de montos hay más fraudes?**  
  🔹 Transacciones fraudulentas suelen estar en el rango de $500 a $3.000.  
- **¿Las transacciones fraudulentas ocurren más en ciertos horarios?**  
  🔹 Alta incidencia de fraudes en el horario comercial y la medianoche.  

### 3️⃣ **Visualización de Datos**
- Histogramas y boxplots de montos de fraude vs. transacciones legítimas.
- Gráficos de barras con la distribución de fraudes por tipo de transacción.
---

## 🏁 Conclusiones

🔹 **Patrón de Fraude Identificado**  
- Proporción de Fraude: El gráfico muestra que el 5% de las transacciones totales son fraudulentas, lo que destaca la importancia de identificar y prevenir el fraude.

- Patrón principal: El análisis revela tres patrones principales de fraude:

- Rangos de montos: El gráfico muestra que los montos entre 2500 y 3000 presentan la mayor proporción de transacciones fraudulentas, alcanzando un 6.2%. Le siguen los rangos de 4500 (4.6%) y 500 (5.8%). Esto sugiere que los estafadores pueden estar enfocándose en transacciones de mayor valor, aunque también se observa actividad fraudulenta en montos más bajos.
- Horarios: El gráfico muestra una concentración de actividad fraudulenta entre las 10 a.m. y las 12 p.m., con un pico a las 11 a.m. (8.6%). También se observa un aumento en la actividad fraudulenta entre las 6 p.m. y las 8 p.m., aunque en menor medida. Esto sugiere que los estafadores pueden estar aprovechando las horas de mayor actividad transaccional.
- Tipos de transacción: El gráfico muestra que las transferencias son el tipo de transacción con mayor incidencia de fraude, representando el 5% del total de transacciones. Las compras y los retiros también presentan un número significativo de fraudes, aunque menor que las transferencias

📌 **Siguientes pasos:**  

- Implicaciones: Este patrón sugiere que los estafadores pueden estar utilizando estrategias para identificar y aprovechar las transacciones de mayor valor durante las horas de mayor actividad y la vulnerabilidad de las transferencias. Esto podría indicar la necesidad de mejorar los sistemas de detección de fraude en tiempo real y fortalecer la vigilancia durante estos períodos y para este tipo de transacciones específicas.
- Recomendaciones:
Implementar medidas de seguridad reforzadas para transacciones entre 2500 y 3000, como la autenticación de dos factores o la verificación de identidad.
Aumentar la vigilancia y el monitoreo de transacciones entre las 10 a.m. y las 12 p.m., especialmente para montos entre 2500 y 3000.
Desarrollar modelos de detección de fraude más sofisticados que consideren la combinación de monto, horario y tipo de transacción, así como otras variables relevantes.
Implementar medidas de seguridad adicionales para transferencias, como límites de monto, verificación de beneficiarios y alertas de transacciones sospechosas.
Educar a los usuarios sobre cómo protegerse contra el fraude, especialmente en transacciones de alto valor, durante las horas de mayor riesgo y al realizar transferencias.

---

📦 mi-proyecto  
│-- 📂 data                 # Datos originales y procesados  
│   │-- transacciones.csv    # Datos en bruto  
│   │-- fraude_limpio.csv    # Datos limpios con fraudes  
│   │-- fraude_por_monto.csv # Segmentación por montos  
│-- 📂 notebooks             # Análisis en Jupyter/Colab  
│   │-- fraude_analisis.ipynb # Notebook con análisis exploratorio  
│-- 📂 images               # Gráficos generados  
│   │-- fraude_horarios.png  # Imagen con fraudes por hora  
│   │-- fraude_montos.png    # Imagen con fraudes por monto  
│-- README.md               # Documentación del proyecto 

