# pryecto_sprint2

10/ Dec
Se realizó reunión del equipo de trabajo donde se realizó una presentación de los participantes,
Se revisarón los puntos requeridos por el Sprint a presentar,
Se distribuyeron los temas a trabajar por cada miembro del equipo, definiendo lo siguiente:

Diego: Se encarga del manejo del repositorio, coordinación de reuniones y temas pendientes y la sección de servicios.
Sebastian: Se encarga de realizar lo correspondiente a la cabecera y sección noticias 1.
Nicolas: Se encarga de realizar lo correspondiente a las secciones de equipos y footer.

Dado que es un proyecto académico sin fines comerciales la propiedad intelectual pertenece a los tres integrantes del equipo y no se generan acuerdos/pactos de confidencialidad de la información contenida en el proyecto.

11/Dec
Se crea el repositorio y el proyecto en GitHub con los Issues correspondientes a cada uno de acuerdo con lo pactado en la reunión del equipo. 

12/Dec
Se coordina reunión con el tutor asignado donde se presenta el equipo, se habla acerca de la dinámica de trabajo y se tratan los temas generales correspondientes al Sprint.

14/Dec
Se hace seguimiento a avances en los Isuues y el el trabajo asignado a cada uno.

15/Dec
Se van finalizando la entregas por cada uno de los integrantes del equipo y se realiza la integración en la rama de desarrollo.

16/Dec
Pruebas finales y se realuza  la entrega a la rama master con el proyecto terminado.

#Documentación

##Bootstrap

Para el desarrollo de la aplicación se utilizaron los siguientes componentes de Bootstrap:

######Navbar El header principal de la aplicación utilizado tiene los enlaces a cada una de las divisiones del proyecto utilizando como referencia el identificador de la clase.

######Carrousel Este carrousel se utiliza como la primera sección de  la página y es adaptada de los ejemplos principales de la documentación.

######Form Utilizando form-group y otras clases se provee el estilo gráfico al formulario cuya lógica se implementa con emailjs

##API
La sección de noticias hace uso del API mediastack para obtener la información de interés. Para esto utilizamos una cuenta gratuita que permite 200 consultas con el token provisto, se utiliza un filtrado que toma noticias relativamente recientes, con fuentes de cnn y bcc para la palabra clave "spacex"

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your unit tests
```
npm run test:unit
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

