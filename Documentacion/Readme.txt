# MEDICION Y EVALUACION DE LA CALIDAD ACADEMICA CON PROYECCION DEL RENDIMIENTO ESTUDIANTIL 
EN UNA UNIDAD EDUCATIVA MEDIANTE MODELOS DE SERIES DE TIEMPO

Este proyecto forma parte del Diplomado en Ciencia de Datos V3 y tiene como objetivo evaluar la calidad
academica, diseñar y evaluar modelos de aprendizaje automatico para la prediccion del rendimiento academico
en una unidad educativa median el uso de modelos de series de tiempo: **XGBoost** y **RandomForest**

#Instrucciones para la Reproduccion

1. **Entrar a la carpeta "Codigos"**:
	Aqui se encuentran todos los codigos para preparar los datasets necesarios, para replicar
	los resultados en caso de querer trabajar con el dataset ya preparado para el analisis de este
	ejecutar los notebooks correspondientes a los modelos cambiando la ubicacion de los datasets
	en el codigo.
	En caso se quiera ejecutar el modelo en un nuevo dataset se tiene que ejecutar el codigo py
	"preparar_dataset_notas_dobleheader_2024" remplazando la gestion correspondiente en el nombre,
	detro el codigo se tiene que remplazar la ubicacion del registro de notas y de los 24 
	centralizadores de notas correspondientes a la gestion que se quiera incorporar, todos los archivos
	tienen que estar formato en xlsx o csv, el programa py guardara como resultado un dataset de la
	gestion correspondiente en formato xlsx y csv, cambiar la ubicacion de la carpeta de acuerdo
	a donde se quiera guardar.

2. **Limpiar la columna nombres de los estudiantes**
	Los datasets preparados anteiormente se tienen que eliminar los nombres antes de usarlos para
	realizar los analisis y modelados correspondientes para eso se tiene que ejecutar el archivo
	"Analisis", se recomiendo realizarlo en google colab, el codigo guardar el dataset sin nombres
	en formato csv listo para ejecutar los notebooks de los modelos.

3. **Ejecutar los notebooks en orden**
	Todos los notebooks estan numerados y contienen **comentarios detallados** en cada celda 
	explican el proceso a seguir.

4. **Proyectar trimestre**
	Dentro de ambos notebooks existo un bloque de codigo que proyecta un trimestre, para proyectar
	determinado trimestre se tiene que modificar el numero de trimestre requerido(1 o 2 o 3) en caso
	se requiera proyectar una gestion completa el modelo RandomForest tiene un bloque especificamente
	para ese tipo de casos, solo hay que modificar el numero de la gestion pensada.

5. **Analisis Estadistico**
	Para un analisis de una gestion determinada se tiene que copiar cualquiera de los dashboards como
	"Gestion2024" con nombre y remplzar la carga de datos por un csv de la gestion a analizar, es 
	obligatorio que el nuevo dataset tenga la misma cantidad y los mismos nombres de cada variable
	caso contrario el dashboard no reconocera los datos y no podra mostrar ningun resultado estadistico
	para su posterior analisis.
	Para un analisis de proyecciones se tiene el dashboard "graficos de proyecciones", lo unico que se
	tiene que hacer es cargar el dataset de la gestion proyectada y agregarla al dataset general que
	utiliza el dashboard en power bi, se recomienda revisar tutoriales para realizarlo 