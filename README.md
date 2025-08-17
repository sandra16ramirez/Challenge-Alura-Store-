# Alura Store – Proyecto de Data Science

**Desafío**: Analizar el desempeño de cuatro tiendas (Alura Store) para determinar cuál debería cerrarse, utilizando datos de facturación, satisfacción del cliente, costos operativos y mix de productos. Proyecto desarrollado en el reto de Alura Latam.

---

##  Contenido del Repositorio

- `notebook.ipynb`: Jupyter Notebook con todo el análisis paso a paso, gráficos y conclusiones.
- Datos importados desde enlaces públicos (`tienda_1.csv` hasta `tienda_4.csv`).
- Visualizaciones clave:
  - Facturación total por tienda (gráfico de barras).
  - Facturación por categoría para cada tienda (gráfico apilado).
  - Calificación promedio por tienda (gráfico de barras horizontales).
  - Costo de envío promedio (gráfico de pie).
- Informe final en Markdown dentro del notebook con recomendación de cierre.

---

##  Objetivo

Ayudar al Sr. Juan —propietario de las tiendas— a decidir cuál cerrar, enfocándose en:
- Maximizar ingresos.
- Mejorar la satisfacción del cliente.
- Optimizar costos logísticos.
- Reasignar recursos a unidades con mayor potencial.

---

##  Metodología

1. Carga de los datos desde archivos CSV.
2. Cálculo de métricas clave:
   - **Facturación total**: suma de `Precio` por tienda.
   - **Facturación por categoría**: `groupby("Categoría del Producto").sum("Precio")`.
   - **Calificación promedio**: media aritmética de la columna `Calificación`.
   - **Costo de envío promedio**: media aritmética de `Costo de envío`.
3. Extracción de productos más y menos vendidos por tienda.
4. Visualización con `matplotlib`:
   - Comparaciones claras y etiquetadas.
5. Interpretación y recomendación final: cierre de la **Tienda 4** por desempeño inferior comparativo.

---

##  Conclusión y Recomendación

- **Recomendación final**: cerrar la **Tienda 4**.
  - Tiene la facturación más baja.
  - Su calificación no supera a las demás.
  - Aunque su envío es más barato, eso no compensa su menor rendimiento general.
- Estrategia sugerida:
  1. Reorientar marketing e inventario hacia Tiendas 1 y 3.
  2. Replicar eficiencias logísticas de la Tienda 4 en otras tiendas.
  3. Desarrollar una campaña de redirección de clientes con beneficios para facilitar la transición.
  4. Monitorear indicadores clave por 60–90 días tras el cierre y reasignación.

---
