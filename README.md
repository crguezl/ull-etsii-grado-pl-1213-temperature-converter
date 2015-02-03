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

para procesar `tests/test.html` y convertirlo a JavaScript.
Ejecución:

          ~/srcPLgrado/temperature(karma2)]$ node_modules/karma/bin/karma start
