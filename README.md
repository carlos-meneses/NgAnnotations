# NgAnnotations

## Lo que puedo declarar en una vista A2

* ***Propiedades:*** Cualquier valor que podemos asignar por medio de un atributo del HTML. 
Ese elemento puede ser simplemente un atributo del HTML estándar, un atributo implementado 
mediante el propio Angular 2 o un atributo personalizado, creado para un componente en específico.

* ***Expresiones:*** Es un volcado de cualquier información en el texto de la página, como contenido 
a cualquier etiqueta {{value}}. La expresión es una declaración que Angular procesará y sustituirá por su valor, 
pudiendo realizar pequeñas operaciones.

* ***Binding:*** Es un enlace entre el modelo y la vista. Mediante un binding si un dato cambia en el modelo,
ese cambio se representa en la vista. Pero además en Angular se introduce el "doble binding", por el cual si un valor 
se modifica en la vista, también viaja hacia el modelo.

* ***Eventos:*** es un suceso que ocurre y para el cual se pueden definir manejadores, que son funciones que se 
ejecutarán como respuesta a ese suceso.

## Flujo de los datos de acuerdo a los elementos Angular 2 que declaramos en la vista

* ***Propiedades:*** Las propiedades tienen un flujo desde el modelo a la vista. Una información disponible en 
el modelo se puede asignar como valor en un elemento del HTML mediante una propiedad, usando la notación corchetes. 
**Por ej: [propiedad]**

* ***Expresiones:*** Las expresiones también viajan desde el modelo a la vista. La diferencia de las propiedades 
es que en este caso las usamos como contenido de un elemento y además que se expresan con dobles 
llaves. **Por ej: {{expresión}}**

* ***Binding:*** El binding (a dos sentidos, o doble binding) lo expresamos entre corchetes y paréntesis. 
En este caso la información fluye en ambos sentidos, desde el modelo a la vista y desde la vista al 
modelo. **Por ej: [(ngBind)]**

* ***Eventos:*** Los eventos no es que necesariamente hagan fluir un dato, pero sí se considera un flujo de aplicación, 
en este caso de la vista al modelo, ya que se originan en la vista y generalmente sirven para ejecutar métodos que 
acabarán modificando cosas del modelo. **Por ej: (evento)**