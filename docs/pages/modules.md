Los módulos hacen referencia a las funcionabilidades de la aplicación.

Un módulo declara un contexto de compilación para un conjunto de componentes que está dedicado a un dominio de aplicación,
flujo de trabajo o un conjuto de capacidades estrechamente relacionadas.
En un módulo podemos asociar componentes,directivas,pipes,etc.
Organizar el código en distintos módulos funcionales ayuda a gestionar el desarrollo de aplicaciones complejas
, y en el diseño para su reutilización.Además esta técnica te permite aprovechar el lazy loading, es decir cargar modulos
solo cuando sea necesario para minimizar la cantidad de código que debe cargar al inicio.

Por ejemplo:
Si la aplicación está orientada a realizar citas médicas.
    - Un módulo seria de citas médicas donde podriamos añadir citas médicas, editar, eliminar,etc.
    - Otro módulo seria el de médicos donde podriamos hacer las mismas acciones mencioanadas anteriormente.

Entonces el folder quedaria asi.



    ├── src
    │   ├── app
    │   │   ├── modules 
    │   │   │   │   ├──citas-medicas
    │   │   │   │   │
    │   │   │   │   │    ├── pages
    │   │   │   │   │    │   ├── citas-medicas-home
    │   │   │   │   │    │   │        ├── citas-medicas.component.ts
    │   │   │   │   │    │   │        ├── citas-medicas.component.html
    │   │   │   │   │    │   │        ├── citas-medicas.component.scss 
    │   │   │   │   │    │   │        ├── citas-medicas.component.spec
    │   │   │   │   │    │   ├── agregar-citas-medicas
    │   │   │   │   │    │   │        ├── agregar-citas-medicas.component.ts
    │   │   │   │   │    │   │        ├── agregar-citas-medicas.component.html
    │   │   │   │   │    │   │        ├── agregar-citas-medicas.component.scss 
    │   │   │   │   │    │   │        ├── agregar-citas-medicas.component.spec
    │   │   │   │   │    │
    │   │   │   │   ├──medicos
    │   │   │   │   │    │
    │   │   │   │   │    ├── pages
    │   │   │   │   │    │   ├── medicos-home
    │   │   │   │   │    │   │        ├── medicos.component.ts
    │   │   │   │   │    │   │        ├── medicos.component.html
    │   │   │   │   │    │   │        ├── medicos.component.scss 
    │   │   │   │   │    │   │        ├── medicos.component.spec
    │   │   │   │   │    │   ├── agregar-medicos
    │   │   │   │   │    │   │        ├── agregar-medicos.component.ts
    │   │   │   │   │    │   │        ├── agregar-medicos.component.html
    │   │   │   │   │    │   │        ├── agregar-medicos.component.scss 
    │   │   │   │   │    │   │        ├── agregar-medicos.component.spec
    
    

 
