# 🪙 Cripto vs. el Peso Argentino

Análisis histórico del comportamiento de Bitcoin y Ethereum en el contexto macroeconómico argentino, con foco en la evolución de los precios en pesos y su relación con el tipo de cambio oficial.

---

## 📊 Dashboard

![Página 1 - Panorama General](screenshots/pagina1.png)
![Página 2 - Cripto en Pesos](screenshots/pagina2.png)
![Página 3 - Análisis de Tendencia](screenshots/pagina3.png)

---

## 🎯 Objetivo

Responder una pregunta concreta: **¿Cómo se comportaron Bitcoin y Ethereum medidos en pesos argentinos a lo largo de los últimos 10 años?**

El proyecto cruza datos históricos de precios de criptomonedas con los tipos de cambio del Banco Central para analizar el impacto de las sucesivas devaluaciones del peso sobre el valor de los activos digitales.

---

## 📁 Estructura del proyecto

```
crypto-vs-peso-arg/
├── 📓 crypto_vs_peso_arg.ipynb     ← Limpieza y transformación de datos
├── 📊 dashboard.pbix                ← Dashboard interactivo en Power BI
├── 📁 data/
│   ├── btc-usd-max.csv              ← Historial BTC/USD (CoinGecko)
│   ├── eth-usd-max.csv              ← Historial ETH/USD (CoinGecko)
│   └── tipos-de-cambio-historicos.csv ← Tipos de cambio BCRA
├── 📁 screenshots/
│   ├── pagina1.png
│   ├── pagina2.png
│   └── pagina3.png
└── 📄 README.md
```

---

## 🔧 Herramientas utilizadas

| Herramienta | Uso |
|-------------|-----|
| Python 3 + Pandas | Limpieza y transformación de datos |
| Jupyter Notebook | Exploración y documentación del proceso |
| Power BI Desktop | Visualización e dashboard interactivo |

---

## 📐 Proceso de datos

El notebook `crypto_vs_peso_arg.ipynb` documenta todo el proceso:

1. **Carga** de los 3 datasets crudos
2. **Limpieza** — parseo de fechas, renombre de columnas, eliminación de duplicados
3. **Exploración** — análisis de valores nulos, rangos temporales y tipos de dato
4. **Transformación** — merge de datasets, cálculo de precios en ARS, retornos diarios y promedios móviles
5. **Exportación** — generación del CSV limpio para Power BI

---

## 📈 Páginas del dashboard

### Página 1 — Panorama General
Evolución histórica de BTC y ETH en dólares desde 2013, con KPIs de máximos y mínimos históricos y segmentador por rango de fechas.

### Página 2 — Cripto en Pesos ⭐
La página más diferenciadora del proyecto. Muestra el precio de BTC y ETH convertido a pesos argentinos usando el tipo de cambio oficial, evidenciando el impacto de las devaluaciones sobre el valor de los activos.

### Página 3 — Análisis de Tendencia
- **Promedios móviles** de 30 y 200 días sobre el precio de BTC
- **Retorno diario promedio por año** — identifica claramente los ciclos alcistas (2013, 2017, 2020) y bajistas (2018, 2022)
- **Scatter plot** de correlación entre retornos diarios de BTC y ETH

---

## 💡 Hallazgos principales

- Bitcoin llegó a valer más de **$178 millones de pesos argentinos** en su pico histórico (2025)
- El salto brusco en el tipo de cambio de **diciembre 2023** se refleja claramente en el precio de ambas criptomonedas en ARS
- Los retornos de BTC y ETH muestran una **correlación positiva** — ambos activos tienden a moverse en la misma dirección
- Los años bajistas del mercado cripto (**2018 y 2022**) son claramente identificables en el análisis de retorno diario promedio

---

## 📦 Fuentes de datos

- **CoinGecko** — historial de precios BTC/USD y ETH/USD
- **BCRA (Banco Central de la República Argentina)** — tipos de cambio históricos

---

## 👤 Autor

**Tomás Carranza**  
Data Analyst | Córdoba, Argentina  
[LinkedIn](https://linkedin.com/in/tcarranza001) · [GitHub](https://github.com/carranzaTomas001)
