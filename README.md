<div align="center">

# 📡 TelecomX
# Análisis de Evasión de Clientes (Churn)

![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

</div>

---

# 📌 ¿De qué trata este proyecto?

TelecomX enfrenta un problema crítico: **el 26.6% de sus clientes abandona el servicio**. Esto significa que 1 de cada 4 clientes se va, generando pérdidas directas de ingresos y altos costos de reemplazo.

Este proyecto aplica un proceso completo de **ELT + Análisis Exploratorio de Datos** para responder una pregunta clave:

> *¿Qué factores llevan a un cliente a abandonar el servicio y cómo podemos prevenirlo?*

---


## 🚨 Resultado Principal

<div align="center">

| Métrica | Valor |
|---------|-------|
| 👥 Total de clientes analizados | 7.032 |
| ❌ Clientes que evadieron | 1.869 |
| ✅ Clientes retenidos | 5.163 |
| 📉 Tasa de evasión | **26.6%** |

</div>

---

## 🔍 ¿Qué encontramos?

Los factores con mayor impacto en la evasión fueron:

**📋 Tipo de Contrato**
- Clientes **mes a mes** evaden al **42.7%**
- Clientes con contrato de **dos años** solo evaden al **2.8%**

**🌐 Servicio de Internet**
- **Fibra óptica** presenta la tasa más alta con **41.9%**
- Posiblemente relacionado con expectativas de precio vs calidad

**💳 Método de Pago**
- **Cheque electrónico** concentra el **45.3%** de evasión
- Métodos automáticos como tarjeta de crédito bajan al **15.3%**

**🕐 Antigüedad del Cliente**
- Los clientes que evaden llevan en promedio **18 meses**
- Los retenidos llevan en promedio **37.7 meses**
- El período más crítico son los **primeros 12 meses**

**💰 Cargo Mensual**
- Evadidos pagan en promedio **$74.44**
- Retenidos pagan en promedio **$61.31**

---

## 👤 Perfil del Cliente en Riesgo

```
✗ Contrato mes a mes
✗ Servicio de fibra óptica
✗ Pago por cheque electrónico
✗ Antigüedad menor a 12 meses
✗ Cargo mensual sobre el promedio
✗ Sin servicios adicionales contratados
✗ Adulto mayor
```

---

## 🗂️ Estructura del Repositorio

```
📦 telecomx-analisis
 ┣ 📓 TelecomX_LATAM.ipynb      → Notebook con el análisis completo
 ┣ 🗃️ TelecomX_Data.json        → Dataset original
 ┗ 📋 README.md
```

---

## 🛠️ Proceso Aplicado

```
📥 Carga del JSON        →   Estructura anidada con 4 bloques
🔧 Aplanado              →   pd.json_normalize() por bloques
🧹 Limpieza              →   Nulos, strings vacíos, tipos de datos
🌐 Traducción            →   Columnas y valores al español
📊 Análisis              →   Visualizaciones por cada factor
💡 Conclusiones          →   Perfil de riesgo + recomendaciones
```

---

## 💡 Recomendaciones Clave

| # | Acción | Impacto Esperado |
|---|--------|-----------------|
| 1 | Incentivar contratos largos con descuentos | Alto |
| 2 | Programa de onboarding primeros 12 meses | Alto |
| 3 | Revisar propuesta de valor de fibra óptica | Alto |
| 4 | Migrar clientes a pagos automáticos | Medio |
| 5 | Pruebas gratuitas de servicios adicionales | Medio |
| 6 | Atención diferenciada para adultos mayores | Medio |

---


<div align="center">

*Proyecto desarrollado con fines de análisis estratégico de retención de clientes*

</div>
