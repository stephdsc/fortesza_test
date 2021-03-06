# Pruebas de automatizaci贸n Fortesza

_Proyecto de automatizaci贸n de pruebas de registro, edici贸n y validaci贸n en la web https://staging.fortesza.com._

## Comenzando 馃殌

_Estas instrucciones te permiten obtener una copia del proyecto en funcionamiento en tu m谩quina local para prop贸sitos de desarrollo y pruebas._

### Pre-requisitos 馃搵

_驴Que cosas necesitas para instalar el software y como instalarlas?_

```
Nodejs y un IDE de tu gusto.
```

### Instalaci贸n 馃敡

_Sigue el paso a paso que sigue a continuaci贸n, para tener un entorno de desarrollo ejecutandose_

_Descargar la versi贸n recomendada de nodejs en la web oficial_

```
https://nodejs.org/es/
```

_Ejecutar el siguiente comando dentro del proyecto copiado localmente_

```
npm install
```

### Ejecutando las pruebas 鈿欙笍

_Para correr las pruebas automatizadas en tu ambiente local ejecuta la siguiente instrucci贸n_

```
npm run test
```

### Interactive shell para resguardar contrase帽as y correos 鈱笍

_Ejecutar las siguientes instrucciones en el terminal donde ejecutaste el script de pruebas para interactuar con las contrase帽as y correos para el registro de un nuevo usuario e inicio de sesi贸n_

_Registro de nuevo usuario_

```
fillField('#txt-email', 'usuario@dominio.com');
```
```
fillField('#txt-password', 鈥楾est1234__#.');
```
```
fillField('#txt-confirm-password', 'Test1234__#.'');
```

_Inicio de sesi贸n_

```
fillField('//input[@formcontrolname="password"]', 'contrase帽aActual');
```

_Edici贸n de contrase帽a en perfil de usuario_


```
fillField('//input[@formcontrolname="password"]', 'contrase帽aAnterior');
```

```
fillField('//input[@formcontrolname="confirmPassword"]', 'nuevaContrase帽a');
```

_Indicar adicionalmente que para salir del terminal interactivo y continuar con el test se debe escribir el comando exit en el terminal, ejemplo:_

```
I.exit
```

### Analice las pruebas end-to-end 馃敥

_Luego de ejecutarse el paso a paso de la prueba automatizada se generara un reporte en formatos HTML y JSON dentro del proyecto para analizar las pruebas_

```
[mochawesome] Report JSON saved to /Users/****/****/auto-test/mochawesome-report/mochawesome.json
```
```
[mochawesome] Report HTML saved to /Users/****/****/auto-test/mochawesome-report/mochawesome.html
```

## Construido con 馃洜锔?

_Herramientas utilizadas para crear el proyecto_

* [Codeceptjs](https://codecept.io/puppeteer/) - El framework web usado
* [Npm](https://docs.npmjs.com/) - Manejador de dependencias
* [Mochawesome](https://www.npmjs.com/package/mochawesome/) - Usado para generar reportes

## Autor 鉁掞笍

* **Stephanie Soteldo** - *Prueba t茅cnica - Parte 2: Automatizaci贸n* - [stephdsc](https://github.com/stephdsc)

## Licencia 馃搫

Este proyecto est谩 bajo la Licencia (Mi Licencia) - mira el archivo [LICENSE.md](LICENSE.md) para detalles

---
馃捇 con 馃挐 por [stephdsc](https://github.com/stephdsc) 馃懇馃徎鈥嶐煉?
