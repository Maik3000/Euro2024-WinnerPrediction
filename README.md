# 🏆 Euro 2024 - Análisis y Predicción de Probabilidades de Victoria

Este proyecto tiene como objetivo principal **estimar qué selecciones nacionales tienen más probabilidades de ganar la Eurocopa 2024**, basándonos en datos cuantitativos como el valor de mercado y la experiencia internacional de los jugadores de cada país. 

Para lograr este objetivo, primero se realizó un análisis de **clustering no supervisado** con el fin de visualizar agrupamientos de países basados en características similares, como el **Market Value** y las **International Caps**. Este clustering permitió obtener una visión más clara sobre qué países tienen mayor valor de mercado y cuáles tienen más experiencia, lo que luego fue utilizado para generar las **Probabilidades de Victoria**.

---

## 🎯 Objetivo

- Realizar un análisis de Clustering para agrupar países en términos de **valor de mercado** y **experiencia internacional**.
- Calcular un índice de **valor de mercado promedio** por selección.
- Calcular un índice de **experiencia internacional** (Total Caps) por selección.
- Estimar una **probabilidad de victoria relativa** para cada país en función de los dos índices anteriores.
- Visualizar los resultados de forma clara y ordenada.

---

## 🧠 Modelos de Clustering Aplicados

El análisis comenzó con un paso de **clustering** utilizando varios algoritmos para identificar agrupamientos de países basados en sus características. Esto ayudó a entender mejor qué selecciones están en situaciones similares en cuanto a su valor de mercado y experiencia:

| Modelo      | Silhouette Score |
|-------------|------------------|
| **K-Means** | 0.434 ✅ (Mejor desempeño) |
| MeanShift   | 0.298            |
| DBSCAN      | 0.297            |

> **Silhouette Score** mide qué tan bien separados están los clusters: cuanto más cercano a 1, mejor.


---

## 📊 Indicadores Usados

- **`country_marketValue`**: Índice basado en el valor de mercado promedio de los jugadores de cada país.
- **`Country_experience`**: Índice basado en la cantidad total de partidos internacionales disputados (Caps).
- **`Winning Probability`**: Estimación proporcional basada en la suma ponderada de los índices anteriores.


---

## 📈 Anexos

- 📊 Tableau Dashboard: https://public.tableau.com/app/profile/mayco.castellanos/viz/EuroPlayersTableau/EuroDashboard
- ✍️ Medium Article: https://medium.com/@maycocastellanos/who-will-win-euro-2024-prediction-from-data-science-4760519bdc1f

---

## ⚙️ Tecnologías y Librerías

- Python 3.x
- pandas
- matplotlib
- scikit-learn
- seaborn

---

**Autor:** Mayco Castellanos  
