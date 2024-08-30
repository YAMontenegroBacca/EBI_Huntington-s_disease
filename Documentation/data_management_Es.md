### Versión Español 
# Data Management
Con el fin de asegurar la integridad y calidad de los datos obtenidos y manipulados, así como la transparencia y reproducibilidad de los análisis realizados, se ha desarrollado el siguiente protocolo para el manejo de los datos:

## Tipos de Datos a manejar:
- **Datos Primarios**: Corresponderán a las secuencias genéticas de obtenidas bases de datos públicas.
- **Datos Secundarios**: Corresponderán a los resultados de análisis y procesamiento de las secuencias obtenidas utilizando herramientas del EBI (European Bioinformatics Institute).
- **Metadatos**: Cada dato (primario o secundario) debe contener información contextual sobre las secuencias descargadas.
 - **Primarios:** fuente, fecha de descarga, parámetros de búsqueda, filtros empleados
 - **datos de análisis (Secundarios):** herramientas y versiones utilizadas, parámetros de análisis.
- **Documentación:** Esta corresponde a una carpeta especifica en la que se describe el proyecto, incluyendo el protocolo de gestión de datos, el archivo README, y otros documentos relevantes

## Almacenamiento:
Los datos manejados en entre proyecto se estarán almacenando y compartiendo en el repositorio de GitHub: [link repositorio](https://github.com/YAMontenegroBacca/EBI_Huntington-s_disease.git)
A continuación, se presenta un ejemplo de la organización del repositorio según las carpetas y archivos ya creados:
-	Documentation 
 - README.md
 - Data_management_Es.md
 - Data_management_En.md
-	Primary_Data
 -	Programmatic_acces
  -	first_search.py
-	Secondary_Data


**Nota:** En cada carpeta se irán almacenando la información correspondiente según las herramientas empleadas. Cada dato generado contiene su respectivo archivo con los metadatos correspondientes. 

## Procesamiento y Análisis de Datos
Para este proyecto, se emplearán las herramientas proporcionadas por el European Molecular Biology Laboratory - European Bioinformatics Institute (EMBL-EBI). Dentro de estas herramientas se encuentran
-	Herramientas de acceso programático
-	Bases de datos: Europe PMC, ENA, EVA y PDBe
-	ENSEMBL
-	Expression Atlas
-	Uniprot
-	AlphaFold
-	Interpro
-	Reactome
-	IntAct

## Principios FAIR 
### Findable (Localizable)
Los datos de gitHub se han organizado empleando nombres fáciles de comprender, cada carpeta en GitHub ha sido creada de tal forma que se pueda comprender la información que contiene. Adicionalmente, cada archivo contiene una descripción breve sobre su finalidad y descripción de datos de entrada, salida y parámetros requeridos para su ejecución.
Los datos secundarios, es decir los datos generados luego del empleo de las herramientas de análisis, deberán contener un identificador único para que puedan ser identificadas y accedidas con facilidad y sin confusiones. Finalmente, tanto datos primarios como secundarios deben contar con sus respectivos metadatos con la información descrita en la sección de Tipos de Datos a manejar.
### Accessible (Accesible)
Toda la información del proyecto será constantemente actualizada en el repositorio de GitHub, este es un repositorio público por lo que la información puede ser constantemente accedida sin ninguna restricción. Las herramientas y resultados que se generarán en el proyecto serán de acceso libre para que no haya limitaciones en su uso o revisión.
### Interoperable (Interoperable)
Los datos obtenidos y generados tendrán formatos estándar que pueden ser accedidos por diferentes sistemas, plataformas y herramientas. Los formatos generalmente empleados serán FASTA, CSV o TSV, JSON o XML, en cada tipo de dato generado se describirá el formato de entrada y de salida para limitar los problemas de uso de los datos. Además, se empleará un lenguaje claro, se empleará ontologías y las descripciones generales serán generadas en Español e inglés para que sea de fácil comprensión.  
### Reusable (Reutilizable)
Los datos serán generados asegurando que contengan la información necesaria para comprender tanto su obtención como su generación, de esta forma nos aseguramos de que puedan ser empelados posteriormente por diferentes personas. En algunos casos a los documentos se adjuntarán pantallazos que indiquen los resultados que se han ido generando, esto ya que con el tiempo las plataformas empleadas pueden cambiar y una imagen de la versión que se está empleando puede ayudar a comprender mejor el proceso llevado a cabo.
