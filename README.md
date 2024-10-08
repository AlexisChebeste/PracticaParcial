# Preparación para el Parcial - Ejercicios JavaScript

Este repositorio contiene una serie de ejercicios clave para el parcial de la materia **Construcción de Interfaces de Usuario**. A continuación se incluyen los 10 ejercicios trabajados, junto con las explicaciones y anotaciones fundamentales a tener en cuenta.

---

## Ejercicio 1: Filtrar Productos
### Descripción:
Función `filtrarProductos` que filtra productos por categoría y precio dentro de un rango dado.

### Conceptos clave:
- **`filter()`**: Ideal para crear un array nuevo con elementos que cumplan una condición.
- **Uso de condicionales**: Verificar la categoría y el rango de precios.

### Buenas prácticas:
- Usar `filter()` cuando se quiere obtener un subconjunto de elementos.
- Mantener las condiciones claras y en una sola línea si es posible.

---

## Ejercicio 2: Ordenar Empleados
### Descripción:
Función `ordenarEmpleados` que aplica un aumento salarial a empleados mayores de 30 años y ordena el array por salario de mayor a menor.

### Conceptos clave:
- **`map()`**: Para aplicar transformaciones a los elementos de un array sin modificar el original.
- **`sort()`**: Para ordenar arrays, en este caso por salario en orden descendente.

### Buenas prácticas:
- Usar `map()` para modificar objetos dentro de un array, sin cambiar el array original.
- En el `sort()`, devolver un número negativo, positivo o 0 para establecer el orden.

---

## Ejercicio 3: Gestionar Tareas
### Descripción:
Función `gestionarTareas` que filtra tareas no completadas y cuya fecha límite no haya pasado.

### Conceptos clave:
- **`filter()`**: Para obtener tareas no completadas.
- **Objeto `Date`**: Para comparar fechas límite y verificar si una fecha ha pasado.

### Buenas prácticas:
- Al trabajar con fechas, usar siempre el objeto `Date` para evitar problemas de comparación de strings.
- Verificar siempre el formato de la fecha (YYYY-MM-DD) antes de usar `Date`.

---

## Ejercicio 4: Carrito de Compras
### Descripción:
Implementación de un carrito de compras con los métodos `agregarProducto`, `eliminarProducto`, y `calcularTotal`.

### Conceptos clave:
- **Operaciones en arrays**: Para añadir, eliminar y sumar productos.
- **Funciones personalizadas**: Crear funciones específicas para cada acción del carrito.

### Buenas prácticas:
- Usar `find()` para encontrar si un producto ya existe antes de agregarlo.
- Modularizar las funciones, de manera que cada una cumpla con una tarea específica.

---

## Ejercicio 5: Analizar Texto
### Descripción:
Función `analizarTexto` que cuenta cuántas veces aparece cada palabra en un texto largo, excluyendo palabras comunes.

### Conceptos clave:
- **`split()`**: Para dividir el texto en palabras.
- **`reduce()`**: Para contar la frecuencia de las palabras en un objeto.

### Buenas prácticas:
- Limpiar el texto antes de procesarlo (conversión a minúsculas, eliminación de puntuación).
- Utilizar un objeto para almacenar la frecuencia de las palabras.

---

## Ejercicio 6: Agrupar por Departamento
### Descripción:
Función `agruparPorDepartamento` que agrupa empleados por departamento y los ordena por salario de mayor a menor.

### Conceptos clave:
- **Agrupación de objetos**: Usar objetos clave-valor para agrupar elementos.
- **Ordenación dentro de un grupo**: Usar `sort()` para ordenar empleados por salario.

### Buenas prácticas:
- Crear un objeto donde las claves sean los nombres de los departamentos y los valores arrays de empleados.
- Separar la lógica de agrupación de la lógica de ordenación para mantener el código limpio.

---

## Ejercicio 7: Listado de Precios (Menús)
### Descripción:
Funciones para calcular el precio promedio de los ítems del primer menú y para actualizar el precio de un ítem en el segundo menú.

### Conceptos clave:
- **`reduce()`**: Para sumar precios y calcular el promedio.
- **Manipulación de arrays**: Para actualizar los precios mediante su índice.

### Buenas prácticas:
- Usar `reduce()` para cálculos agregados como el promedio.
- Trabajar con referencias a los elementos del DOM para actualizar la interfaz.

---

## Ejercicio 8: Calculadora
### Descripción:
Script de una calculadora que realiza operaciones matemáticas entre dos números y muestra el resultado en una etiqueta `div`.

### Conceptos clave:
- **Eventos (`click`)**: Para ejecutar una función al presionar el botón de calcular.
- **Manipulación del DOM**: Para mostrar el resultado en tiempo real.

### Buenas prácticas:
- Capturar y manejar los eventos `click` de manera eficiente.
- Validar las entradas del usuario (números válidos) antes de realizar cualquier cálculo.

---

## Ejercicio 9: Validación de Formulario en Tiempo Real
### Descripción:
Formulario con campos de texto y número que valida los datos en tiempo real. Si un campo está vacío al intentar enviar, muestra un mensaje de error.

### Conceptos clave:
- **Eventos `input` y `submit`**: Para validar en tiempo real y al intentar enviar.
- **Manipulación del DOM**: Mostrar y ocultar mensajes de error debajo de los campos.

### Buenas prácticas:
- Usar eventos `input` para validar conforme el usuario escribe.
- Prevenir el envío de formularios inválidos con `event.preventDefault()` en el `submit`.

---

## Ejercicio 10: Buscador de Precios
### Descripción:
Buscador de precios que recibe el nombre de un producto y muestra su precio. Si el producto no existe, muestra un mensaje de error.

### Conceptos clave:
- **`find()`**: Para buscar el producto dentro de una lista de productos.
- **Manipulación del DOM**: Mostrar el precio o mensaje de error en la página.

### Buenas prácticas:
- Convertir las entradas del usuario a minúsculas para evitar errores por diferencias en el uso de mayúsculas/minúsculas.
- Mostrar mensajes claros de éxito o error en la interfaz de usuario.

---

## Notas adicionales para el parcial
- **Manipulación del DOM**: Tener claro cómo seleccionar, modificar y actualizar elementos del DOM es fundamental.
- **Métodos de arrays**: El uso correcto de `filter()`, `map()`, `reduce()`, y `sort()` es clave para manipular datos.
- **Funciones reutilizables**: Mantener las funciones pequeñas y específicas. Evitar funciones que realicen múltiples tareas.
- **Eventos y validación**: Comprender cómo funcionan los eventos y cómo hacer validaciones en tiempo real es esencial para crear interfaces dinámicas y robustas.

---
