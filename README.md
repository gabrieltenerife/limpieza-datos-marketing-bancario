# Análisis y Limpieza de Datos: Campaña de Marketing Bancario

Este repositorio contiene un tutorial práctico desarrollado en Python utilizando la librería Pandas, enfocado en el preprocesamiento, limpieza y tratamiento inicial de un conjunto de datos procedente de una campaña de marketing de una entidad bancaria.

## Objetivo del Negocio
El proyecto busca responder a una pregunta clave dentro del sector financiero: ¿Qué perfil tienen los clientes con mayor potencial de aceptar un depósito a término ofrecido mediante llamadas telefónicas?

Para lograr esto, el primer paso fundamental es garantizar la integridad, calidad y consistencia de los datos antes de pasar a fases posteriores como el análisis exploratorio (EDA) o la modelización.

## Estructura del Dataset
El conjunto de datos original (`dataset_banco.csv`) cuenta con 45,215 registros y 17 columnas, divididos en:
* **Variables Demográficas y Laborales:** Edad, tipo de trabajo, estado civil y nivel educativo.
* **Variables Financieras:** Saldo promedio anual, historial de impagos (`default`), créditos hipotecarios y de consumo (`housing`, `loan`).
* **Variables de Interacción:** Medio de contacto, día, mes, duración de la llamada, número de contactos en la campaña actual (`campaign`), días transcurridos desde campañas anteriores (`pdays`), número de contactos previos (`previous`) y resultado de las campañas pasadas (`poutcome`).
* **Variable Objetivo (`y`):** Indica si el cliente se suscribió o no al producto (`yes`/`no`).

## Proceso de Limpieza y Preprocesamiento
En este script se abordan las problemáticas más comunes en la ingeniería de datos:
1. **Gestión de valores nulos:** Identificación e imputación o eliminación estratégica de registros incompletos en variables clave.
2. **Revisión de columnas irrelevantes:** Verificación de variabilidad en las características para asegurar que todas aporten valor analítico.
3. **Control de duplicados:** Limpieza de filas repetidas para evitar sesgos.
4. **Detección y tratamiento de Outliers:** Análisis estadístico y visualización mediante diagramas de caja (boxplots) para identificar valores atípicos (como edades erróneas o duraciones negativas) y decidir su tratamiento sin perder información valiosa.
5. **Normalización de variables categóricas:** Detección de errores tipográficos y unificación de subniveles equivalentes.

## Tecnologías Utilizadas
* Python
* Pandas (Manipulación y limpieza de estructuras tabulares)
* Matplotlib y Seaborn (Visualización de datos y detección de anomalías)
