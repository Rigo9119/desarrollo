# HTML Study notes

Hyper Text Markup Language 

No es un lenguaje de programación, es un lenguaje de hipermarcado,
en desarrollo web es lo que le de la estructura a las paginas / apps

como todo lenguaje tien sentencias y para escribirlas necesitamos tags

```html
<html></html>
````

la mayoria de tags tienen una apertura y un cierre, otros tags como img son 
self close y tambien tienen atributos como src o alt los que van a contener 
algun valor

```html
<img src="" alt=""/>
```

## Versiones 

La ultima version es la 5 y es progresiva(salen verisones como en js)
se escribe con html! y la mayoria de ides van formatear el documento

## Estructura

Todos los documentos html tienen una estructura compuesta de tags
"principales" doctype, html, head, body.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

Doctype es lo que le que le dice al buscador que version de html se
esta usando

html encierra toda la estructura que va tener la app

head contiene la metadata e informacion necesaraia de la pagina y 
para el buscador

body es lo que contiene la estructura visual de la pagina/app

## Estilos y Scripts

Los estilos y scripts de la pagina se pueden incluir de varias maneras

Styles -> se pueden incluir en el head con el tag style 
```html
<head>
  <style>
    * {
      box-sizing: border-box;
    }
  </style>
</head>
```
O tambien se pueden incluir de forma "inline"
```html
<h1 style="font-size: 16px;"></h1>
```

La idea en general es separar estos en sus respectivos archivos .css o 
.scss

Los scrips al igual que los estilos se pueden incluir en el head pero por 
lo general se ubican al final del body, pero la idea es que tambien tengan
sus archivos .js
```html
<head>
  <script></script>
</head>
```
```html
<body>
  <script></script>
</body>
```

la diferencia es que al ubicarlo en el head pueden haber conflictos con los
estilos ya que el buscador carga de arriba hacia abajo, siguiendo esa idea 
la estructura cargaria de ultimo y si hay manipulacion del dom puede tener
conflictos

## HTML Semantico

Escribir html semantico significa darle mas significado al documento html 
esto con el fin de desarrollar para gente que tiene alguna discapacidad,
para esto se deberian seguir ciertos puntos.

  * utilizar tags que le den sentido a la estructura del documento, 
    por ejemplo utilizar el tag head para el header, nav para los
    menus, footer, y los diferentes headers para los titulos

  * tambien se debe incluir el atributo alt en todas las imagenes
    para poder mostrar la descripcion de la imagen 

  * utilizar lenguaje conciso para los links y botones

  * utilizar ARIA tags para screen readers

## Lazy loading
TO-DO 
