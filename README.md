beta.adalab.es/modulo-1-evaluacion-final-mhbeatriz/

# Evaluación de Beatriz Mendoza Huertas

Esta es mi evaluación final sobre el módulo 1 de Adalab, en la que he puesto a prueba los siguientes conocimientos y aptitudes sobre maquetación con HTML y CSS:

Por un lado;

- He usado una estructura ordenada de ficheros y carpetas, los cuales están enlazados con sus respectivos ficheros.

En cuanto a la maquetación con HTML:

- Todo el código está perfectamente indentado.
- La sintáxis y semántica está estructurada desde mi criterio, de una manera fácil de entender.

Respecto a la maquetación con CSS/Sass:

- Todo el código está perfectamente indentado.
- He dividio el Sass en varios partials para que me resulte más cómodo y ordenado, y los he enlazado correctamente el fichero principal.
- He creado otro fichero a parte para las variables, en las cuales he añadido la paleta de colores y la tipografía que se pide para luego enlazarlas comodmente en cada clase.

La estructura de carpetas tiene esta pinta:

src
├─ api // los ficheros de esta carpeta se copian en public/api/
| └─ data.json
├─ images
├─ scss
| ├─ components
| ├─ core
| ├─ layout
| └─ pages
└─ html
└─ partials

- La mayor parte de la página web esta maquetada con flex.
- Con el objetivo de dotar de dinamismo a la página y hacerlo más interactiva he añadido algunas transiciones a los botones, los cuales, están enlazados tanto de forma relativa como absoluta.

# Agradecimientos

## Guía de inicio rápido

> **NOTA:** Necesitas tener instalado [Node JS](https://nodejs.org/) para trabajar con este Starter Kit:

### Pasos a seguir cada vez que queremos arrancar un proyecto desde cero:

1. **Crea tu propio repositorio.**
1. Descarga este **Starter kit desde GitHub**.
   - No recomendamos que clones este repo ya que no podrás añadir commits.
1. **Copia todos los ficheros** de este Starter kit en la carpeta raíz de tu repositorio.
   - Recuerda que debes copiar **también los ficheros ocultos**.
   - Si has decidido clonar este repo, no debes copiar la carpeta `.git`. Si lo haces estarás machacando tu propio repositorio.
1. **Abre una terminal** en la carpeta raíz de tu repositorio.
1. **Instala las dependencias** locales ejecutando en la terminal el comando:

```bash
npm install
```

### Pasos para arrancar el proyecto:

Una vez hemos instalado las dependencias, vamos a arrancar el proyecto. **El proyecto hay que arrancarlo cada vez que te pongas a programar.** Para ello ejecuta el comando:

```bash
npm start
```

Este comando:

- **Abre una ventana de Chrome y muestra tu página web**, al igual que hace el plugin de VS Code Live Server (Go live).
- También **observa** todos los ficheros que hay dentro de la carpeta `src/`, para que cada vez que modifiques un fichero **refresca tu página en Chrome**.
- También **procesa los ficheros** HTML, SASS / CSS y JS y los **genera y guarda en la carpeta `public/`**. Por ejemplo:
  - Convierte los ficheros SASS en CSS.
  - Combina los diferentes ficheros de HTML y los agrupa en uno o varios ficheros HTML.

Después de ejecutar `npm start` ya puedes empezar a editar todos los ficheros que están dentro de la carpeta `src/` y programar cómodamente.

### Pasos para publicar el proyecto en GitHub Pages:

Para generar tu página para producción ejecuta el comando:

```bash
npm run docs
```

Y a continuación:

1. Sube a tu repo la carpeta `docs/` que se te acaba de generar.
1. Entra en la pestaña `settings` de tu repo.
1. Y en el apartado de GitHub Pages activa la opción **master branch /docs folder**.
1. Y ya estaría!!!

Además, los comandos:

```bash
npm run push-docs
```

o

```bash
npm run deploy
```

son un atajo que nos genera la versión de producción y hace push de la carpeta `docs/` del tirón. Te recomendamos ver el fichero `package.json` para aprender cómo funciona.

## Flujo de archivos con Gulp

Estas tareas de Gulp producen el siguiente flujo de archivos:

![Gulp flow](./gulp-flow.png)

## `gulpfile.js` y `config.json`

Nuestro **gulpfile.js** usa el fichero `config.json` de configuración con las rutas de los archivos a generar / observar.

De esta manera separarmos las acciones que están en `gulpfile.js` de la configuración de las acciones que están en `config.json`.
