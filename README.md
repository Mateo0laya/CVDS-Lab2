# CVDS-Lab2

## **Apache Maven**

Es una herramienta de comprensión y gestión de proyectos de software. Maven puede administrar la construcción, los informes y la documentación de un proyecto desde una pieza central de información.
El resultado es una herramienta que ahora se puede usar para construir y administrar cualquier proyecto basado en Java.
Maven se basa en el concepto central de un ciclo de vida de construcción. Lo que esto significa es que el proceso para construir y distribuir proyecto está claramente definido.

### Fases de Maven

>Cada uno de estos ciclos de vida de construcción está definido por una lista diferente de fases de construcción, donde una fase de construcción representa una etapa en el ciclo de vida.

1) Validate: validar que el proyecto sea correcto y que toda la información necesaria esté disponible
2) compile: compilar el código fuente del proyecto
3) Test: probar el código fuente compilado utilizando un marco de prueba de unidad adecuado. Estas pruebas no deberían requerir que el código sea empaquetado o implementado.
4) Package: tomar el código compilado y empaquetarlo en su formato distribuible, como un JAR.
5) Verify: ejecutar cualquier verificación de los resultados de las pruebas de integración para garantizar que se cumplan los criterios de calidad.
6) Install: instalar el paquete en el repositorio local, para usarlo como dependencia en otros proyectos localmente.
7) Deploy- Realizado en el entorno de compilación, copia el paquete final en el repositorio remoto para compartirlo con otros desarrolladores y proyectos.

### Ciclo de vida de Maven

>Hay tres ciclos de vida de compilación integrados:

1) Default: maneja la implementación del proyecto.
2) Clean: maneja la limpieza del proyecto.
3) Site: maneja la creacion del sitio web del proyecto.

### Plugins

>Los plugins son artefactos que proporcionan objetivos a Maven. Además, un plugin puede tener uno o más objetivos en los que cada objetivo representa una capacidad de ese plugin. Los complementos pueden contener información que indica a qué fase del ciclo de vida vincular un objetivo. Tenga en cuenta que agregar el complemento por sí solo no es suficiente información; también debe especificar los objetivos que desea ejecutar como parte de su compilación.

### Repositorio central de Maven

El repositorio central de Maven es la ubicación predeterminada para que Maven descargue todas las bibliotecas de dependencia del proyecto para su uso. Para cualquier biblioteca involucrada en el proyecto, Maven primero busca en la carpeta .m2 del Repositorio local, y si no encuentra la biblioteca necesaria, busca en el Repositorio central y carga la biblioteca en el repositorio local.
El repositorio de Maven (o repositorio central) tiene una estructura que permite que los archivos como, por ejemplo, archivos JAR tengan versiones distintas que se descubren después fácilmente con un mecanismo de denominación bien conocido. A continuación, las herramientas de creación pueden utilizar estos nombres para extraer dinámicamente las dependencias de la aplicación. En la definición de la aplicación que se denomina archivo POM, cuando se utiliza Maven como una herramienta de compilación, simplemente denomine las dependencias y el proceso de compilación sabrá qué hacer a partir de ahí.


## Crear un proyecto con Maven
