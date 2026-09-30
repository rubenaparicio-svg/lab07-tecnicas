# Tarea: Mi prompt avanzado

## Tarea elegida

Diseño e implementación de un módulo de gestión de calificaciones y promedios ponderados en Java.

---

## Versión 1: Prompt básico

Crea un programa en Java para calcular el promedio de notas de un estudiante.

## Version 2

<rol>Actúa como arquitecto de software especializado en Java.</rol>
<contexto>Módulo para un sistema de gestión académica escolar.</contexto>
<tarea>Diseña una clase Java que calcule el promedio ponderado de un estudiante considerando el peso porcentual de cada evaluación.</tarea>
<formato>Código Java estructurado con buenas prácticas de POO y comentarios Javadoc.</formato>

## Version 3: prompt final

<rol>Actúa como Líder Técnico en Java y Especialista en Control de Calidad de Software (QA).</rol>
<contexto>
Sistema universitario donde las notas están en el rango de 0.0 a 20.0 y cada evaluación tiene un peso porcentual asociado. La suma de los pesos de las evaluaciones debe ser exactamente igual al 100%.
</contexto>
<tarea>

1. Razona paso a paso cómo calcular el promedio ponderado validando casos límite (notas fuera de rango 0-20, suma de pesos diferente de 100% y listas de evaluaciones vacías).
2. Genera el código Java completo de la clase GestionNotas con manejo defensivo de excepciones.
3. Aplica autocrítica: Revisa si tu código maneja adecuadamente las excepciones IllegalArgumentException y agrega 3 casos de prueba unitarios utilizando JUnit 5.
   </tarea>
   <ejemplos>
   Ejemplos de formato de salida deseado:

- Error de rango -> "Error: La nota 22.0 está fuera del rango permitido [0.0 - 20.0]"
- Registro exitoso -> "Estudiante: Juan Pérez | Promedio Ponderado: 16.5"
  </ejemplos>
  <formato>
  Responde en Markdown con bloques de código `java`, tablas comparativas para la autocrítica y comentarios explicativos en cada método.
  </formato>

## Técnicas usadas en el prompt final

| Parte del Prompt Final           | Técnica Aplicada        | Propósito / Beneficio en la Respuesta                                                         |
| -------------------------------- | ----------------------- | --------------------------------------------------------------------------------------------- |
| `<rol>...</rol>`                 | **Role Prompting**      | Asigna el perfil de Líder Técnico/QA para exigir estándares altos de código y pruebas.        |
| `<ejemplos>...</ejemplos>`       | **Few-shot**            | Define la estructura sintáctica exacta para las respuestas de éxito y manejo de errores.      |
| `1. Razona paso a paso...`       | **Chain of Thought**    | Obliga a la IA a procesar la lógica de negocio y casos borde antes de escribir el código.     |
| `<rol>`, `<contexto>`, `<tarea>` | **Prompt Estructurado** | Organiza las instrucciones en secciones claras etiquetadas evitando ambigüedades.             |
| `3. Aplica autocrítica...`       | **Autocrítica**         | Fuerza a la IA a revisar su propia respuesta y complementar con pruebas unitarias en JUnit 5. |

---

## Evaluación del resultado

| Criterio de Evaluación                                                          | Cumple (Sí / No) |
| ------------------------------------------------------------------------------- | ---------------- |
| ¿Tiene un rol específico y formato definido?                                    | Sí               |
| ¿Incluye validación defensiva para notas fuera de rango (0-20) y suma de pesos? | Sí               |
| ¿Aplica al menos tres técnicas de prompting combinadas?                         | Sí               |
| ¿Genera pruebas unitarias JUnit 5 tras el proceso de autocrítica?               | Sí               |

---

## Por qué elegí estas técnicas

Elegí combinar **Role Prompting**, **Prompt Estructurado**, **Chain of Thought**, **Few-Shot** y **Autocrítica** porque el desarrollo de software requiere máxima precisión técnica y cobertura de pruebas. El rol de Líder Técnico/QA establece el nivel de exigencia; el prompt estructurado separa claramente la tarea del contexto; la cadena de pensamiento garantiza la verificación previa de casos borde lógicos; los ejemplos fijan el formato de salida; y la autocrítica permite identificar y corregir omisiones de código o pruebas unitarias antes de finalizar la respuesta.

- [Tarea: mi prompt avanzado](prompts/TAREA.md)
