# Proyecto 5 – Análisis de Embudo de Eventos y Test A/A/B

## 📋 Descripción general
Este proyecto analiza el comportamiento de usuarios dentro de una aplicación digital, evaluando su conversión a lo largo del embudo de eventos y los resultados de un experimento A/A/B.  
El objetivo es entender los puntos de abandono, medir el rendimiento de las versiones y determinar si los cambios aplicados tienen un impacto significativo en la conversión.

---

## 🎯 Objetivos
- Construir un embudo de conversión por pasos.
- Calcular las tasas de conversión y puntos críticos de abandono.
- Analizar los resultados del experimento A/A/B y verificar la homogeneidad de los grupos.
- Aplicar pruebas estadísticas para determinar diferencias significativas.
- Formular recomendaciones para mejorar la experiencia del usuario.

---

## 🧮 Datos utilizados
**Archivo:** `logs_exp_us.csv`  
Columnas principales:
- EventName: Nombre del evento (MainScreenAppear, OffersScreenAppear, etc.)
- DeviceIDHash: ID del usuario.
- EventTimestamp: Fecha y hora del evento.
- ExpId: Grupo experimental (246 y 247 → A/A, 248 → B).

Periodo analizado: aproximadamente 1–3 meses.  
Muestra estimada: entre 200k y 300k eventos.

---

## 🧰 Herramientas y librerías
- Python
- pandas, numpy, matplotlib, seaborn, scipy
- Jupyter Notebook
- Git / GitHub

---

## 📊 Etapas del análisis
1. Limpieza y preprocesamiento de datos.
2. Identificación de usuarios únicos y grupos experimentales.
3. Construcción del embudo de conversión.
4. Cálculo de tasas de conversión entre pasos.
5. Comparación de grupos A/A y A/B.
6. Pruebas estadísticas de significancia (Mann–Whitney U Test).
7. Visualización de resultados y conclusiones.

---

## 🔍 Resultados principales
- Los grupos A/A (246 y 247) mostraron resultados estadísticamente similares, validando el experimento.
- El grupo B (248) presentó una mejora del 3% en conversión total, pero sin significancia estadística (p > 0.05).
- La mayor pérdida de usuarios se observó entre los pasos “OffersScreenAppear” y “CartScreenAppear”.
- Los datos reflejan una experiencia de usuario consistente entre versiones.

---

## 📈 Métricas clave
- Conversión grupo A: 47.3 %
- Conversión grupo B: 50.2 %
- Diferencia relativa: +2.9 %
- p-value: 0.08
- Usuarios analizados: ~7,500 por grupo

---

## 💡 Conclusiones y recomendaciones
- Mantener el diseño actual: no hay evidencia significativa de mejora.
- Ampliar la muestra y repetir el experimento para aumentar potencia estadística.
- Investigar el abandono entre ofertas y carrito.
- Analizar la segmentación por tipo de usuario o canal de adquisición.

---

## 🗂 Estructura del repositorio
