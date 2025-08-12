Pasos para implementación.

Descomprimir contenido de zips en workspace de Eclipse
- ms_ordenes		(App Spring boot)
- camel-integration     (App Spring boot)

Descomprimir contenido de zip en algun directorio con proyectos .NET:
- OrdenesAPI		(.NET API)

Descomprimir contenido de zip en directorio con proyectos Angular:
- proyecto-angular	(angular)

Se debe actualizar las dependncias maven en ambos proyectos Spring Boot

Iniciar proyecto ms_ordenes desde IDE Eclipse como run AS "Spring boot App".
Iniciar proyecto camel-integration desde IDE Eclipse como run AS "Spring boot App".
Iniciar proyecto OrdenesAPI desde Visual Studio 2022 

camel-integration:
	- En carpeta "logs" se registran los envios procesados.

ms_ordenes
	- En carpeta "logs" se encuentran los registros procesados.

IMPORTANTE:
Se debe ajustar la ruta del archivo para servicio .NET API

Achivo: ArchivoOrdenesService.cs

private static string rutaArchivo = @"C:\Users\SONY\eclipse-workspace\camel-integration\data\inbox\ordenes.json";
Se debe cambiar a donde se haya alojado el proyecto de Spring (camel-integration), manteniendo la parte camel-integration\data\inbox\ordenes.json.
de esta manera se podra traspasar el archivo entre servicios.

