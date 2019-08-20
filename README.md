# the-ultimate-redux-implementation

Miren, para cambiar un poco el hilo y no hablar de una implementación específica de state management. Lo que queremos en el front es estado compartido. Hoy en día, aplicaciones grandes que tienen diversos componentes, necesitan mantener estado en común, como por ejemplo, los items de un carro.

Un componente los necesitará para calcular el precio, otro los impuestos, otro componente los va a necesitar para mostrar un resumen al usuario de lo que está comprando, otro para mostrar un popup de vista rápida al carro, etcétera.

Sin estado compartido, estos componentes deberían conseguirlo de una api en tiempo real, lo cual es extremadamente ineficiente y potencialmente lleva a inconsistencias.

Ahora, si reducimos todo el "fuzz" y los features extra de los frameworks de state management, lo que nos queda son tres funcionalidades básicas, sencillamente implementables por uno mismo.

1. Setear estado
2. Actualizar estado
3. Escuchar por cambios de ese estado

Esto es todo. No necesitas más para hacer state management. Redux, Vuex y otros frameworks similares, implementan toda una clase de conceptos externos que complejizan innecesariamente lo que sucede en el core, es decir, estas tres acciones básicas que acabo de mencionar.

Es por no comprender estas tres acciones básicas, pienso yo, que muchas aplicaciones se "van de las manos".
