	
El Core Module es responsable de mantener los servicios globales. Por ejemplo los servicios HTTP para comunicarse con una API. También se utiliza para almacenar guards, modelos y otras dependencias globales, como el interceptor http y el controlador de errores global. Para mantener una base de código bien estructurada y escrita
El Core Module agrupa “componentes” que sí y sólo si se van a compartir a través de toda la aplicación pero generando una referencia única.

El core debe contener instancias donde solo hay una por aplicación.


*   Guards: Son servicios especiales que ayuda a otorgar acceso a rutas.
*   Interceptores: Ayudan a interceptar o modificar las solicituds y respuestas http.
*   Modelos: Deberíamos poner modelos generales en el módulo.
*   Servicios: Servicios para realizar las peticiones htpp.
*   Componentes: Contendrá los componentes que son comunes en toda la aplicación, como encabezado, footer,barra de navegación.
