# AI Log - XGBros

## Herramientas
- Claude (claude.ai)
- Google Gemini

## Registro de uso

### 2026-04-11 | Gemini | Procesamiento de los datos. 

- **Tarea**: Limpiar y preparar los conjuntos de datos del Coneval 'pobreza22.csv'. Se necesitaba manejar valores nulos, convertir tipos de datos y normalizar variables.
- **Resultado**: Gemini generó un script robusto utilizando scikit-learn y pandas que incluía un SimpleImputer para los valores nulos y un StandardScaler para las variables numéricas.
- **Modificación**: Ajustamos el script para excluir columnas de metadatos, ya que el modelo intentaba procesarlas como variables predictoras innecesarias.

### 2026-04-11 | Gemini | Mapa interactivo

- **Tarea**: Generar un mapa de la República Mexicana que muestre el grado de carencia en salud por estado, utilizando un degradado de color para identificar zonas críticas.
- **Resultado**: Proporcionó el código usando plotly.express y nos ayudó a encontrar un archivo GeoJSON con los estados de México para vincularlo con nuestro DataFrame de pandas.
- **Modificación**: Ajustamos la escala de colores para que los colores rojos representen una carencia mayor y los verdes una menor carencia en salud.

### 2026-04-11 | Claude | Conversión de las gráficas a Quarto.

- **Tarea**: Migrar las visualizaciones generadas en plotly a un reporte de Quarto (.qmd).
- **Resultado**:  Claude tradujo el código a formato plotly.graph_objects para hacerlo interactivo, además de agregar recuadros con estadísticas interesantes (promedio de ingreso nacional).
- **Modificación**: Se integraron parámetros de layout para un diseño visual más agradable.
