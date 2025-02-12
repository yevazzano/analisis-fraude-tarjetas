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
  🔹 (Ejemplo: Transacciones fraudulentas suelen estar en el rango de $500 a $3.000.  
- **¿Las transacciones fraudulentas ocurren más en ciertos horarios?**  
  🔹 Alta incidencia de fraudes en el horario comercial y la medianoche.  

### 3️⃣ **Visualización de Datos**
- Histogramas y boxplots de montos de fraude vs. transacciones legítimas.
- Gráficos de barras con la distribución de fraudes por tipo de transacción.

---

## 🏁 Conclusiones

🔹 **Patrón de Fraude Identificado**  
_(Aquí puedes resumir las principales conclusiones de tu análisis, por ejemplo: los fraudes ocurren más en ciertos horarios, ciertos tipos de transacciones o en rangos de montos específicos)._  

📌 **Siguientes pasos:**  
_(Opcional: puedes mencionar si piensas aplicar modelos de Machine Learning o algún otro análisis adicional)._

---

## 📂 Estructura del Proyecto

