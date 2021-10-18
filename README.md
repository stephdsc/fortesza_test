# Pruebas de automatización Fortesza

_Proyecto de automatización de software para automatizar pruebas de registro, edición y validación en la web https://staging.fortesza.com._

## Comenzando 🚀

_Estas instrucciones te permiten obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._

### Pre-requisitos 📋

_¿Que cosas necesitas para instalar el software y como instalarlas?_

```
Nodejs y un IDE de tu gusto.
```

### Instalación 🔧

_Sigue el paso a paso que sigue a continuación, para tener un entorno de desarrollo ejecutandose_

_Descargar la versión recomendada de nodejs en la web oficial_

```
https://nodejs.org/es/
```

_Ejecutar el siguiente comando dentro del proyecto copiado localmente_

```
npm install
```

### Ejecutando las pruebas ⚙️

_Para correr las pruebas automatizadas en tu ambiente local ejecuta la siguiente instrucción_

```
npm run test
```

### Interactive shell para resguardar contraseñas y correos ⌨️

_Ejecutar las siguientes instrucciones en el terminal donde ejecutaste el script de pruebas para interactuar con las contraseñas y correos para el registro de un nuevo usuario e inicio de sesión_

_Registro de nuevo usuario_

```
fillField('#txt-email', 'usuario@dominio.com');
```
```
fillField('#txt-password', ‘Test1234__#.');
```
```
fillField('#txt-confirm-password', 'Test1234__#.'');
```

_Inicio de sesión_

```
fillField('//input[@formcontrolname="password"]', 'contraseñaActual');
```

_Edición de contraseña en perfil de usuario_


```
fillField('//input[@formcontrolname="password"]', 'contraseñaAnterior');
fillField('//input[@formcontrolname="confirmPassword"]', 'nuevaContraseña');
```

### Analice las pruebas end-to-end 🔩

_Luego de ejecutarse el paso a paso de la prueba automatizada se generara un reporte en formatos HTML y JSON para analizar las pruebas_

```
Los reportes se guadan en la carpeta mochawesome-report
```

## Construido con 🛠️

_Herramientas utilizadas para crear el proyecto_

* [Codeceptjs](https://codecept.io/puppeteer/) - El framework web usado
* [Npm](https://docs.npmjs.com/) - Manejador de dependencias
* [Mochawesome](https://www.npmjs.com/package/mochawesome/) - Usado para generar reportes

## Autor ✒️

* **Stephanie Soteldo** - *Prueba técnica - Parte 2: Automatización* - [stephdsc](https://github.com/stephdsc)

## Licencia 📄

Este proyecto está bajo la Licencia (Mi Licencia) - mira el archivo [LICENSE.md](LICENSE.md) para detalles

---
💻 con 💝 por [stephdsc](https://github.com/stephdsc) 👩🏻‍💻
