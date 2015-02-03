ETSII ULL Grado de Informatica
==============================

# Asignatura Procesadores de Lenguajes

## Primera Práctica:

Conversor en JavaScript de grados Celsius a Farenheit y viceversa

## Pruebas

Para Karma es necesario instalar:

* [karma html2js converter](https://github.com/karma-runner/karma-html2js-preprocessor)
* `npm install karma-html2js-preprocessor --save-dev`
* `npm install karma-chrome-launcher --save-dev`
* `npm install karma-firefox-launcher --save-dev`
* [karma html2js converter]([karma phantomJS launcher ](https://github.com/karma-runner/karma-phantomjs-launcher)

En `karma.conf.js` tenemos que poner:

              files: [
                'tests/test.html',
                'tests/*.js',
                'temperature.js'
              ],

y

              preprocessors: {
                    'tests/*.html': ['html2js']
              },

para procesar `tests/test.html` y convertirlo a JavaScript:

          if (typeof __html__ !== 'undefined') { // Que sirva con y sin Karma

Ejecución:

          ~/srcPLgrado/temperature(karma2)]$ node_modules/karma/bin/karma start

You can pass list of browsers as a CLI argument too:

          ~/srcPLgrado/temperature(karma2)]$ node_modules/karma/bin/$karma start --browsers PhantomJS
