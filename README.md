### **Farmland Suitability Analysis — Obafemi Owode LGA, Ogun State, Nigeria**

This project presents a **GIS-based multi-criteria land suitability analysis** developed to identify optimal areas for agricultural expansion within **Obafemi Owode Local Government Area (LGA), Ogun State, Nigeria**.

The analysis integrates terrain, hydrology, soil properties, and accessibility factors to produce a **data-driven farmland suitability model**, supporting informed decision-making for agricultural planning and land acquisition.

---

## **Project Objectives**

* Identify highly suitable farmland zones across the LGA
* Minimize risks associated with flooding and poor drainage
* Evaluate soil conditions for crop productivity
* Incorporate accessibility and irrigation potential into land selection
* Generate actionable spatial outputs for field validation

---

## **Data Sources**

The analysis combines multiple geospatial datasets:

* Digital Elevation Model (DEM)
* LGA boundary data
* SoilGrids data (clay content and soil organic carbon)
* Extracted drainage network (from DEM)
* OpenStreetMap road network
* Derived hydrological layers

---

## **Methodology**

The workflow follows a structured geospatial analysis process:

### 1. Terrain Analysis

* DEM preprocessing (sink filling)
* Slope generation
* Terrain characterization

### 2. Hydrological Modeling

* Flow accumulation
* Stream extraction
* Topographic Wetness Index (TWI)
* Flood-prone area identification

### 3. Soil Analysis

* Depth-weighted aggregation of soil properties (0–30 cm)
* Clay content and soil organic carbon evaluation

### 4. Accessibility & Irrigation

* Distance to road network (logistics suitability)
* Distance to streams (irrigation potential)

### 5. Suitability Modeling

All layers were standardized to a common scale (0–1) and combined using a **weighted overlay approach**:

| Factor          | Description              |
| --------------- | ------------------------ |
| Slope           | terrain suitability      |
| TWI             | soil moisture conditions |
| Flood risk      | environmental constraint |
| Clay            | soil structure           |
| SOC             | soil fertility           |
| Road proximity  | accessibility            |
| River proximity | irrigation potential     |

The result is a **continuous suitability surface** highlighting optimal farmland locations.

---

## **Outputs**

The project produces the following key outputs:

* Slope map
* Topographic Wetness Index (TWI) map
* Flood risk map
* Soil suitability layers
* Road accessibility map
* River proximity map
* **Final farmland suitability map**
* Extracted **prime farmland zones** (top suitability areas)

---

## **Key Insights**

* Suitable farmland is concentrated in **moderately elevated, well-drained areas**
* Floodplains and low-lying zones show **high moisture and risk**
* Soil fertility varies spatially, influencing productivity potential
* Accessibility to roads significantly impacts practical land usability
* Proximity to water sources improves irrigation feasibility

---

## **Tools & Technologies**

* QGIS
* GDAL / GRASS GIS tools
* SoilGrids (global soil database)
* OpenStreetMap (road network data)

---

## **Use Cases**

This analysis supports:

* Agricultural land acquisition
* Farm expansion planning
* Environmental risk assessment
* Spatial decision-making in rural development

---

## **Project Structure**

```
data/           → input datasets  
qgis/           → project files  
maps/           → final outputs and layouts  
docs/           → methodology and documentation  
```

---

## **Author**

Geospatial Analysis Project
Focused on applying GIS techniques for **agricultural planning and land suitability assessment**.

---

## **License**

This project is intended for educational and analytical purposes. Data sources retain their respective licenses.
