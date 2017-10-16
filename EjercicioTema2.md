# Álvaro Carmona Oliva


## 1. Descargar y ejecutar las pruebas de alguno de los proyectos anteriores, y si sale todo bien, hacer un pull request a este proyecto con tests adicionales, si es que faltan (en el momento que se lea este tema).
En el repositorio [siguiente](https://github.com/alvarocarmona6/tdd-gdg) he añadido una función de bisiesto con su correspondiente test para comprobarla.

## 2. Para la aplicación que se está haciendo, escribir una serie de aserciones y probar que efectivamente no fallan. Añadir tests para una nueva funcionalidad, probar que falla y escribir el código para que no lo haga (vamos, lo que viene siendo TDD).
Tanto en el ejercicio anterior como en mi proyecto he utilizado test he probado que fallen y posteriormente lo he arreglado para que pasen los test.

## 3. Convertir los tests unitarios anteriores con assert a programas de test y ejecutarlos desde mocha, usando descripciones del test y del grupo de test de forma correcta. Si hasta ahora no has subido el código que has venido realizando a GitHub, es el momento de hacerlo, porque lo vas a necesitar un poco más adelante.
He utilizado [pocha](https://github.com/rlgomes/pocha), la instalación viene en el enlace anterior. He modificado el test.py del ejercicio 1 con lo siguiente:

        @it('testing sobre la operacion numero bisiesto') 
        def testBisiesto():
        assert Bisiesto(2016) == True

el resultado ha sido el siguiente:
![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/ejercicio3.png)


## 4. Instalar alguno de los entornos virtuales de node.js (o de cualquier otro lenguaje con el que se esté familiarizado) y, con ellos, instalar la última versión existente, la versión minor más actual de la 4.x y lo mismo para la 0.11 o alguna impar (de desarrollo).
He instalado virtualenv y una vez instalado voy a instalar dentro de virtualenv python2.7 y python3.5. El comando utilizado para instalar virtualenv ha sido:

        sudo apt-get install virtualenv python-virtualenv

![captura](https://github.com/alvarocarmona6/Ejercicios-IV/blob/master/capturas/captura4.png)
