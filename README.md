# 🧠 Ejercicio avanzado: TodoApp interactivo con React

En este ejercicio vas a crear una **aplicación de tareas** más completa, donde podrás **añadir tareas nuevas**, **marcarlas como completadas** y **eliminarlas**. Vas a usar `useState`, componentes controlados y funciones que se pasan entre componentes para manejar eventos.

---

### 🎯 Objetivo

Construir una TodoApp funcional con React que permita:

* Ver una lista de tareas
* Añadir nuevas tareas desde un input
* Marcar tareas como completadas
* Eliminar tareas

---

### 📝 Instrucciones

1. **Crea el componente principal `TodoApp`**
   Este será el componente raíz. Dentro de él deberás:

   * Usar `useState` para gestionar el array de tareas
   * Usar otro `useState` para manejar el valor del input controlado

2. **Estructura de una tarea**
   Cada tarea será un objeto con esta forma:

   ```js
   {
     id: 1,
     texto: "Estudiar React",
     completada: false
   }
   ```

3. **Crea un input controlado**
   Añade un formulario con un input de texto y un botón para añadir tareas nuevas. Usa `useState` para controlar el valor del input.

   * Al hacer submit, añade una nueva tarea al array con un `id` único.
   * Borra el input después de añadir la tarea.

4. **Renderiza las tareas con `.map()`**
   Crea un componente `TodoItem` que reciba props:

   * `texto`
   * `completada`
   * `onToggle` → para marcar/desmarcar como completada
   * `onDelete` → para eliminar la tarea

   En `TodoItem`, muestra el texto.

   * Si `completada` es `true`, muestra el texto tachado.
   * Incluye un botón para eliminar la tarea.

5. **Añade lógica en `TodoApp` para manejar eventos**
   Crea funciones que:

   * Marquen una tarea como completada (toggle)
   * Eliminen una tarea
   * Añadan una tarea nueva

   Estas funciones deben pasarse como props a `TodoItem`.

6. **Muestra un mensaje condicional si no hay tareas**
   Si la lista está vacía, muestra el mensaje:
   **"No hay tareas. ¡Agrega una nueva!"**

---

### 💡 Extra (opcional)

* Ordena las tareas: primero las incompletas, luego las completadas.
* Evita añadir tareas vacías (usa `trim()`).
* Muestra un contador de tareas pendientes.

---

¿Listo para el reto? 💪
¡Construye tu TodoApp y deja que React haga su magia!
