# Alimenta Corp: Solución Integral de Business Intelligence

Este repositorio documenta el desarrollo y la implementación de un sistema de Business Intelligence (BI) diseñado para centralizar, transformar y analizar datos operativos de los departamentos de compras y ventas de la empresa Alimenta Corp.

El proyecto abarca el ciclo completo del dato: desde la extracción de fuentes heterogéneas hasta la creación de cubos OLAP y visualizaciones interactivas para la toma de decisiones estratégicas.

## Tecnologías Utilizadas

* **Motor de BD:** Microsoft SQL Server (Transact-SQL).
* **ETL:** SQL Server Integration Services (SSIS).
* **Modelado Multidimensional:** SQL Server Analysis Services (SSAS).
* **Visualización:** Tableau Desktop y Power BI.
* **Entorno de Desarrollo:** Visual Studio 2022 y SQL Server Management Studio (SSMS).

## Arquitectura del Proyecto

El sistema se basa en un diseño de Data Warehouse utilizando un Modelo Estrella (Star Schema), optimizando las consultas para análisis de gran volumen de datos.

### 1. Extracción y Transformación (ETL)
Se implementaron flujos en SSIS para integrar datos provenientes de:
* Bases de datos relacionales (SQL Server y Oracle).
* Archivos planos (.txt) con estructuras de datos legadas.
* **Procesos realizados:** Limpieza de datos nulos, conversión de tipos, tareas de Lookup para integridad referencial y creación de columnas derivadas para lógica de negocio.

### 2. Almacenamiento (Data Warehouse)
Diseño de dimensiones y tablas de hechos:
* **Dimensiones:** Producto, Proveedor, Cliente, Tiempo, Empleado y Sucursal.
* **Tablas de Hechos (Facts):** Ventas y Compras.

### 3. Análisis Multidimensional
Creación de Cubos OLAP en SSAS para permitir análisis de tendencias, comparativas temporales y cálculo de indicadores clave de desempeño (KPIs).

### 4. Visualización de Datos
* **Tableau:** Dashboards dinámicos para el monitoreo de ventas y cumplimiento de metas.
* **Power BI:** Reportes ejecutivos enfocados en el rendimiento operativo y financiero.

## Contenido del Repositorio

Debido a que el proyecto utiliza paquetes binarios y modelos de servidor, este repositorio incluye:
* **/docs:** Documentación Técnica completa en formato PDF detallando cada fase del proyecto.
* **/assets:** Capturas de pantalla de los flujos de control (Control Flow) y flujos de datos (Data Flow) desarrollados en SSIS.
* **/dashboards:** Vistas previas de los tableros interactivos finales presentados a la gerencia.

## Créditos y Colaboración
Proyecto desarrollado para la Facultad de Ingeniería en Sistemas de la Universidad Mariano Gálvez de Guatemala (UMG) por el Grupo No. 3:
* Ronald Yair Ajcac López
* Bill Isaac Méndez Mejicanos
* Héctor Guillermo Rivera Cop
* Juan Carlos García Monroy

## Conclusiones
La implementación logró centralizar información fragmentada, permitiendo detectar áreas de oportunidad y mejorar la eficiencia operativa mediante la automatización de reportes que anteriormente se gestionaban de forma manual.
