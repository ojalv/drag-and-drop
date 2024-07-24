# Explicación

1. **HTML**: Contiene un elemento que se puede arrastrar (`#elemento`) y un contenedor donde se puede soltar (`#contenedor`).

2. **CSS**: Define el estilo de los elementos. El elemento arrastrable tiene un color de fondo verde y el contenedor tiene un borde punteado para indicar el área de destino.

3. **JavaScript**:
   - **`dragstart`**: Se activa cuando el usuario empieza a arrastrar el elemento. Usamos `e.dataTransfer.setData()` para almacenar el ID del elemento.
   - **`dragend`**: Se activa cuando el arrastre termina. Cambiamos el color del elemento para restaurar su estado.
   - **`dragover`**: Se activa cuando el elemento arrastrado está sobre el contenedor. Llamamos a `e.preventDefault()` para permitir que el elemento sea soltado en el contenedor.
   - **`drop`**: Se activa cuando el elemento es soltado en el contenedor. Calculamos la posición donde el elemento debe ser colocado y actualizamos sus propiedades de estilo.

Este es un ejemplo básico que puedes expandir y modificar según tus necesidades. Por ejemplo, puedes añadir más lógica para manejar múltiples elementos, cambiar estilos o mejorar la interacción.
