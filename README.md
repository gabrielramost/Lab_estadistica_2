# **Bienvenidos/as al Laboratorio de Estadística para el Análisis Político 2**

# **1. Objetivos**

El objetivo principal del laboratorio es que los y las participantes desarrollen habilidades básicas e intermedias para la manipulación de datos. Se dotará al estudiante de herramientas para la lectura, limpieza, formateo, integración y visualización de datos, utilizando principalmente el software R y su entorno R Studio.

![](https://github.com/gabrielramost/Lab_estadistica_2/blob/3580b6164af1e82ade74522df80488b1332c55de/Introducci%C3%B3n/datos.jpeg)

**Dinámica de las sesiones**

Las sesiones se realizarán durante 2 horas, teniendo a la mitad del curso un receso de 10 minutos. Se requiere puntualidad del alumno/a, así como respeto y responsabilidad en las actividades. Los horarios y aulas son las siguientes:

- H689A - Sábados de 9:00 a 11:00 en el aula N221 (Edificio McGregor)
- H689B - Sábados de 11:00 a 13:00 en el aula N221 (Edificio McGregor)

La Facultad entregará un certificado de manejo del “Lenguaje R para Análisis Estadístico” a nivel INTERMEDIO al haber obtenido una nota mayor o igual a 14 en cada una de las evaluaciones.


# **2. Requisitos**

## **2.1. Instalación del programa**

Instalar la última versión disponible de R y R Studio: https://posit.co/download/rstudio-desktop/

## **2.2. Configuración de directorio de trabajo**

Recuerden que antes de comenzar a hacer operaciones con R necesitamos definir nuestro lugar de trabajo. Para esto tenemos dos alternativas.

#### **Opción 1. Fijar directorio**

Para ver nuestro lugar de trabajo actual escribimos el siguiente comando:

```{r}
getwd()
```


Para una mejor experiencia, pueden crear una carpeta en la cual trabajá a lo largo del curso. La ruta a través del menú es: **Session > Set Working Directory > Choose Directory**. Esto abrirá una ventana emergente, donde buscaremos la carpeta en la cual vamos a trabajar, la seleccionamos y apretamos "Open".

Si queremos verificar el cambio, volvemos a digitar la función **"getwd()"** en la consola.

#### **Opción 2. Proyecto de R**

Otra opción en crear un proyecto. Al crearlo todos los ficheros quedan vinculados directamente al proyecto. Para crear un proyecto seleccione la ruta: **File > New project...** Se abrirá la siguiente ventana:

![](https://github.com/gabrielramost/Lab_estadistica_2/blob/3580b6164af1e82ade74522df80488b1332c55de/Introducci%C3%B3n/proyecto.png)

Para crear un proyecto en un nuevo directorio, hacemos clic en el botón New Directory. Seguidamente, seleccionamos el tipo de proyecto. Ahora, asignamos un nombre al directorio (carpeta) que se va a crear y que al mismo tiempo será el nombre del proyecto de R. Para terminar, hacemos clic en el botón Create Project. Al seguir este proceso se habrá creado una carpeta en Documentos y un fichero nombre_carpeta.Rproj.

Para crear un proyecto en una carpeta que ya existe, hacemos clic en el botón Existing Directory y después seleccionamos la carpeta ayudándonos del Browse.. si fuera necesario. Una vez elegida la carpeta, clicamos en Create Project.

Para abrir un proyecto hacemos doble clic sobre el archivo con extensión .Rproj o lo abrimos desde el menú de RStudio: File > Open Project...

Ventaja de los proyectos: cualquier fichero que creemos (script de R, documento de Rmarkdown, etc.) y guardemos se guardará en la carpeta del proyecto.


## **2.3. Github**

Vamos a requerir que se creen una cuenta en GitHub. GitHub permite alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. Para fines de este curso, vamos a utilizar Github como repositorio para cargar nuestras bases de datos, administrar nuestros archivos etc.

**Créese una cuenta en Github:**

Ingrese a esta dirección: https://github.com/

Si quiere saber más de GitHub visite:

https://www.youtube.com/watch?v=Uw8SIaAK-vw&t=134s

**Instale Github Desktop**

- Instale https://desktop.github.com/
- Ingrese su usuario y contraseña
- Configure Git (solo con su cuenta Github)

Esta configuración ha creado una carpeta en Documentos, denominada "Github"

**Clone el repositorio del Curso**

Todo el material del curso estará disponible en un repositorio de Github: https://github.com/gabrielramost/Lab_estadistica_2
- Abra el link, seleccione Code, y Open with Github Desktop.
- Luego presione clonar repositorio.
- Con esto podrá visualizar el repositorio en su carpeta de documentos. 
- Para actualizar, siempre que entre a su computador de "Pull origin"

![](https://github.com/gabrielramost/Lab_estadistica_2/blob/3580b6164af1e82ade74522df80488b1332c55de/Introducci%C3%B3n/github.png)


## **2.4. R Markdown**

Vamos a trabajar en archivos R markdown (Rmd). El R Markdown es un lenguaje marcado ligero que nos permite escribir informes que contengan código R . El lenguaje Markdown surge con el objetivo de aligerar las marcas en los lenguajes Markup , principalmente el HTML, pero tambien el LaTeX .En términos sencillos RMarkdown es un procesador de texto que ofrece además la posibilidad de incluir trozos de código desde R (u otros formatos). 

![](https://github.com/gabrielramost/Lab_estadistica_2/blob/3580b6164af1e82ade74522df80488b1332c55de/Introducci%C3%B3n/rmd.png)


Para ejecutar correctamente un documento de RMarkdown y lograr construir un reporte final en el formato deseado, es preciso asegurar que todos estos elementos estén instalados en el computador. Asegurese de instalar adecuadamente los siguientes paquetes (ejecute los siguientes comandos en la consola):

- install.packages(“knitr”)
- install.packages(“tinytex”) 
- tinytex::install_tinytex()


# **3. Comunidad R**

En muchas ocasiones necesitamos ayuda sobre cómo funciona una determinada función, cuáles son sus argumentos, etc.

```{r}
help(mean)
?mean
mean    # y pulsamos la tecla F1
```

Tambien pueden consultar algunas webs que ofrecen ayuda:

+ R Bloggers: <https://www.r-bloggers.com/>
+ Stack Overflow: <https://stackoverflow.com/>

La comunidad de R también está en las redes sociales y es muy activa. 
Pueden usar twitter, instagram y facebook para enterarse de actualizaciones, códigos, etc. Algunas cuentas de twitter interesantes por aquí:

@aRtsy_package: <https://twitter.com/aRtsy_package>
@rfortherest: <https://twitter.com/rfortherest>
@RLangPackage: <https://twitter.com/RLangPackage>
@rstatstweet: <https://twitter.com/rstatstweet>
R Ladies: <https://www.rladies.org/>

Algunos referentes en español:

- Karina Bartolome: <https://karbartolome-blog.netlify.app/posts/tablas-subte/>
- Rossana Ferrero: <https://twitter.com/RosanaFerrero>



