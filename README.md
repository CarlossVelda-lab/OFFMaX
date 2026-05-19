# Efecto de promociones

Aplicación web interactiva para análisis de promociones y descuentos. 

**🌐 Acceso directo:** https://carlossvelda-lab.github.io/promomax/

## Descripción

Esta página web permite:

- ✅ Cargar dos archivos: uno de **ventas** y otro de **promociones**.
- ✅ Aceptar archivos `CSV` o `Excel`.
- ✅ Normalizar columnas clave automáticamente.
- ✅ Convertir descuentos a binario: `1` si hay descuento, `0` si no.
- ✅ Generar gráficos de comparación en tiempo real:
  - Promedio de ingresos con vs. sin descuento
  - Unidades vendidas con vs. sin descuento
  - Comparativas de impacto de promociones
- ✅ Presentar conclusiones locales sin APIs externas

## Características técnicas

- **100% en el navegador** — No requiere servidor backend
- **JavaScript puro** — Procesa archivos CSV y Excel localmente
- **Privacidad** — Los datos no se envían a ningún servidor
- **Gráficos dinámicos** — Chart.js para visualizaciones
- **Responsive** — Funciona en escritorio y móvil

## Cómo usar

1. Accede a: **https://carlossvelda-lab.github.io/promomax/**
2. Carga tu archivo de **ventas** (CSV o Excel)
3. Carga tu archivo de **promociones** (CSV o Excel)
4. Haz clic en **Analizar datos**
5. Visualiza gráficos, métricas e insights

## Estructura de archivos esperados

### Archivo de Ventas
Debe contener columnas como:
- `sku` o `id_producto`
- `precio` (precio unitario)
- `costo`
- `cantidad_vendida`
- `ventas` (ingresos totales, o se calcula automáticamente)
- `categoria`
- `región` o `región`
- `fecha` (fecha de la venta)
- `descuento` (1=sí, 0=no)

### Archivo de Promociones
Debe contener columnas como:
- `sku` o `id_producto`
- `fecha_inicio` (inicio de la promoción)
- `fecha_fin` (fin de la promoción)
- `descuento` (indicador de promoción)

## Archivos del proyecto

- `index.html` — Aplicación web interactiva (GitHub Pages)
- `app.py` — Versión alternativa en Streamlit (opcional)
- `requirements.txt` — Dependencias de Python (si usas Streamlit)
- `.gitignore` — Archivos a ignorar en Git

## Para usar localmente

Si tienes Git instalado:

```bash
git clone https://github.com/CarlossVelda-lab/promomax.git
cd promomax
# Abre index.html en tu navegador
```

## Repositorio

https://github.com/CarlossVelda-lab/promomax
