# DataProject-Proyecto-EDA-con-Python
Proyecto de análisis y tratamiento de datos con Python, trabajando con dos archivos en formatos distintos (CSV y Excel). El objetivo fue limpiar, organizar y combinar ambos datasets para obtener información conjunta sobre clientes de una entidad bancaria portuguesa y su comportamiento frente a campañas de marketing directo.

## Datos
Fuente: proporcionados por el curso/máster
- Archivo de datos en formato CSV: `bank-additional.csv`
- Archivo de datos en formato XLSX: `customer-details.xlsx`

Archivos limpios:
- Archivo de datos en formato CSV: `bnk_add_limpio.csv`
- Archivo de datos en formato CSV: `cust_det_limpio.csv`
- Archivo final combinado mediante merge en formato CSV: `bnk_add_cust_det_merge.csv`
- Archivo final combinado mediante merge en formato XLSX: `bnk_add_cust_det_merge.xlsx`

## Pasos del análisis  
1. Importación de los archivos originales con **pandas**.  
2. Exploración inicial de los datasets por separado para entender su estructura, detectar columnas clave y enfocar el análisis.  
3. Limpieza de datos: tratamiento de nulos y duplicados, conversión de tipos de datos (por ejemplo, fechas) y eliminación de columnas innecesarias.  
4. Creación de nuevas columnas derivadas como `TotalHijos`, `recent_customer` o indicadores de advertencias.  
5. Integración de ambos datasets mediante un **merge**, unificando la información bancaria de los clientes con datos demográficos de los mismos para un análisis más completo.  
6. Aplicación de **filtrados** (ej. clientes de alto ingreso, clientes jóvenes, clientes con llamadas largas).  
7. Realización de **agrupaciones** para obtener estadísticas relevantes (ej. ingresos promedio por año, visitas web según número de hijos, duración de llamadas por profesión).  
8. Representación de resultados mediante **gráficas** como respaldo visual del análisis (en los archivos originales y en el archivo final combinado).

## Conclusiones / Insights  
- Los clientes con **ingresos más altos** tienden a estar concentrados en ciertos años de alta y muestran perfiles familiares más numerosos.  
- La edad promedio varía según el nivel educativo: los clientes con estudios básicos tienden a ser de mayor edad que aquellos con estudios universitarios. Esto tiene sentido ya que antes era más difícil acceder a un nivel educativo más alto como un grado universitario o un grado de formación profesional.  
- La **duración de las llamadas** resulta más elevada en colectivos como estudiantes y jubilados y más bajas cuando se trata de empresarios, lo que podría relacionarse con la disponibilidad de tiempo de cada colectivo.  
- La mayoría de contactos con clientes se llevan a cabo a través de dispositivos móviles frente a una minoría a través de teléfonos fijos. Esto puede apoyar la idea de que la mayoría de clientes se encuentran en edades jóvenes y medias capaces de manejar a la perfección teléfonos móviles mientras que las personas mayores quizás se entiendan mejor con teléfonos fijos.  
- Se detectaron clientes de **riesgo extremo**: mayores de 50 años, con préstamos personales e hipotecarios, y con más de 2 hijos. Este grupo puede requerir una estrategia diferenciada. La gran mayoría de clientes en riesgo extremo se sitúan entre los 50 y los 58 años. Además esta cifra va disminuyendo conforme mayores son los clientes. 
- La mayoría de los clientes tienen entre 30 y 40 años, una edad prudente pero lógica para realizar un depósito a plazo bancario pues no son ni muy jóvenes para pecar de inexperiencia, ni muy mayores para dejarse engañar fruto de malentendidos o confusiones.


## Nota  
En algunas fases del proyecto me he apoyado en la **Inteligencia Artificial** como ayuda puntual, pero siempre como complemento: el trabajo de análisis, limpieza y conclusiones es propio. La sintaxis de las gráficas por el contrario, han sido creadas por la IA pues no tenía conocimientos suficientes para realizarlas por mí mismo.


## Estructura del repositorio  
- `README.md` → este archivo con explicación del proyecto.  
- `Datos_Proyecto_EDA_con_Python` → carpeta con datos brutos (originales) y datos limpios.   
- `Notebooks_Proyecto_EDA_con_Python` → carpeta con los archivos `.ipynb` de los pasos seguidos.
