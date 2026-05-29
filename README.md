# 🎬 Netflix Content Analysis Dashboard
### Análisis exploratorio del catálogo global de Netflix | Tableau Public

![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completado-success?style=for-the-badge)

---

## 📌 Descripción del Proyecto

Dashboard interactivo desarrollado en **Tableau Public** para explorar y analizar el catálogo completo de Netflix: más de **8,780 títulos** distribuidos globalmente. El objetivo fue descubrir patrones en la composición del contenido, su evolución temporal y su distribución geográfica mediante visualizaciones interactivas.

> 🔗 **[[Ver dashboard en Tableau Public](https://public.tableau.com/app/profile/martin.jesus.villon.urday/viz/Libro1_17799839641480/Dashboard1?publish=yes)]
---

## 🖼️ Vista previa

| Dashboard Principal | Dinámicas Temporales |
|---|---|
| ![Dashboard 1](assets/dashboard_01.png) | ![Dashboard 2](assets/dashboard_02.png) |

---

## 📊 Métricas Clave

| Indicador | Valor |
|---|---|
| Total de títulos analizados | **8,780** |
| Películas | **6,120 (69.7%)** |
| Series (TV Shows) | **2,660 (30.3%)** |
| Duración promedio (películas) | **99 minutos** |
| Temporadas promedio (series) | **2 temporadas** |
| Episodios totales (series) | **~4,700** |
| Pico de adiciones anuales | **2020 (+1,200 títulos)** |

---

## 🗂️ Estructura del Dashboard

El proyecto se compone de **8 vistas interconectadas**:

```
Dashboard 1 (Principal)
├── 📍 Mapa          → Distribución geográfica de origen del contenido
├── 📅 Años          → Volumen de contenido añadido por año (2012–2022)
├── 🎭 Tipo          → Composición del catálogo: Movie vs TV Show
├── ⏱️  Duración      → Tabla de métricas por tipo (duración/temporadas)
├── 📈 Dinámica      → Series temporal mensual de adiciones al catálogo
├── 📊 % del Total   → Composición proporcional mes a mes por tipo
├── 🗓️  Date          → Análisis por fecha de adición
└── 🎬 Dato x Años   → Desglose por género (Drama, Comedia) año a año
```

---

## 🔍 Hallazgos Principales

### 1. 🎬 Las películas dominan el catálogo
El **69.7%** del contenido disponible son películas, con una duración promedio de **99 minutos**. Las series, aunque representan el 30.3%, concentran mayor profundidad narrativa con ~4,700 episodios y 2 temporadas en promedio.

### 2. 📈 Explosión de contenido entre 2016 y 2020
El catálogo creció de forma exponencial:
- **2015:** 553 títulos añadidos
- **2017:** 1,028 títulos
- **2019:** 1,028 títulos
- **2020:** +1,200 títulos *(pico máximo)*

Esto refleja la estrategia agresiva de expansión de contenido de Netflix previo y durante la pandemia.

### 3. 🌍 Concentración geográfica en EE.UU.
El mapa interactivo revela que **Norteamérica domina** el origen del contenido:
- 🇺🇸 Estados Unidos: **3,207 títulos**
- 🇮🇳 India: segunda posición con presencia significativa
- 🇬🇧 Europa: distribución secundaria en UK, Francia y España
- 🌎 Latinoamérica: región en crecimiento, aún con baja representación

### 4. 🎭 Drama y Comedia lideran por género
El análisis temporal por género (vista *Dato por Años*) muestra que **Drama** y **Comedia** son las categorías con mayor volumen de contenido añadido año a año, con crecimiento sostenido entre 2018 y 2022.

### 5. 📊 Cambio en la composición proporcional
La vista *Dinámica % del Total* revela que la proporción de **Movies vs TV Shows** no ha sido estática: en ciertos períodos Netflix priorizó series, especialmente a partir de 2018 con el impulso de sus producciones originales.

---

## 🛠️ Stack Tecnológico

| Herramienta | Uso |
|---|---|
| **Tableau Public** | Desarrollo de todas las visualizaciones e interfaz del dashboard |
| **Kaggle - Netflix Dataset** | Fuente de datos principal (8,780+ registros) |
| **Mapbox / OpenStreetMap** | Capa de mapa interactivo para análisis geográfico |
| **Tableau Calculated Fields** | Métricas derivadas y campos calculados dinámicos |
| **Dashboard Actions** | Filtros cruzados e interactividad entre vistas |

---

## 📁 Estructura del Repositorio

```
netflix-tableau-dashboard/
│
├── 📄 README.md                  ← Este archivo
├── 📊 netflix_dashboard.twbx     ← Archivo Tableau (workbook empaquetado)
├── 📂 data/
│   └── netflix_titles.csv        ← Dataset original (Kaggle)
└── 📂 assets/
    ├── dashboard_01.png           ← Captura vista principal
    └── dashboard_02.png           ← Captura vistas dinámicas
```

---

## 🚀 Cómo reproducirlo

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/tu-usuario/netflix-tableau-dashboard.git
   cd netflix-tableau-dashboard
   ```

2. **Abre el workbook**
   - Instala [Tableau Public](https://public.tableau.com/en-us/s/download) (gratuito)
   - Abre el archivo `netflix_dashboard.twbx`

3. **Explora el dashboard**
   - Usa los filtros interactivos para segmentar por tipo, año y género
   - Haz clic en el mapa para filtrar contenido por región
   - Navega entre las 8 hojas de trabajo desde las pestañas

---

## 📚 Dataset

**Fuente:** [Netflix Movies and TV Shows — Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)

| Campo | Descripción |
|---|---|
| `show_id` | Identificador único del título |
| `type` | Movie o TV Show |
| `title` | Nombre del contenido |
| `director` | Director(es) |
| `cast` | Elenco principal |
| `country` | País de origen |
| `date_added` | Fecha de adición al catálogo |
| `release_year` | Año de lanzamiento original |
| `rating` | Clasificación de audiencia |
| `duration` | Duración (minutos o temporadas) |
| `listed_in` | Géneros / categorías |

---

## 👤 Autor

**[Martin Jesus Villon Urday]**
📧 [Urdaymartin27@gmail.com]
🔗 [LinkedIn](www.linkedin.com/in/martin-villon-urday) · [Tableau Public](https://public.tableau.com/app/profile/martin.jesus.villon.urday/viz/Libro1_17799839641480/Dashboard1?publish=yes) · [Portafolio en Notion](https://app.notion.com/p/Portafolio-de-An-lisis-de-Datos-Mart-n-Vill-n-362987249e5280e98159f38d7f3c54d7?source=copy_link)
---

## 📂 Otros proyectos del portafolio

| Proyecto | Herramienta | Descripción |
|---|---|---|
| [RRHH Dashboard](#) | Power BI | Análisis de recursos humanos y rotación de personal |
| [Préstamos Crediticios](#) | Excel / Python | Modelo de riesgo crediticio y análisis de mora |
| **Netflix Content Analysis** | Tableau | Análisis del catálogo global de Netflix ← *este proyecto* |

---

*⭐ Si este proyecto te resultó útil, no olvides dejar una estrella al repositorio.*
