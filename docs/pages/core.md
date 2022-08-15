	
El Core Module es responsable de mantener los servicios globales. Por ejemplo los servicios HTTP para comunicarse con una API. También se utiliza para almacenar guards, modelos y otras dependencias globales, como el interceptor http y el controlador de errores global. Para mantener una base de código bien estructurada y escrita
El Core Module agrupa “componentes” que sí y sólo si se van a compartir a través de toda la aplicación pero generando una referencia única.
