# prompts/BITACORA.md

# Bitácora de técnicas avanzadas

Laboratorio 07: Técnicas Avanzadas de Prompting.
Herramienta de IA usada: ChatGPT (GPT-4o) / Gemini

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo      | Aciertos (de 5) | Formato de la respuesta                                       | Todas con el mismo formato (Sí/No) |
| --------- | --------------- | ------------------------------------------------------------- | ---------------------------------- |
| Zero-shot | 5/5             | Párrafo extenso explicativo por cada comentario               | No                                 |
| One-shot  | 5/5             | Lista numerada con comentario y clasificación                 | No                                 |
| Few-shot  | 5/5             | Estructura estricta en línea: `"Comentario" -> Clasificación` | Sí                                 |

---

## Ejercicio 3: Chain of Thought

| Pedido      | Respuesta de la IA                                                                           | Muestra los pasos (Sí/No) | Correcta (Sí/No) |
| ----------- | -------------------------------------------------------------------------------------------- | ------------------------- | ---------------- |
| Directo     | S/ 318.60                                                                                    | No                        | Sí               |
| Paso a paso | Muestra descuento (120 _ 0.75 = 90), IGV (90 _ 1.18 = 106.20) y total (106.20 \* 3 = 318.60) | Sí                        | Sí               |

---

## Ejercicio 4: Role prompting

| Versión        | Vocabulario (sencillo/técnico) | Usa ejemplos o código                                      | A quién le sirve más                   |
| -------------- | ------------------------------ | ---------------------------------------------------------- | -------------------------------------- |
| A. Sin rol     | Intermedio                     | No usa código, solo definición general                     | Público general                        |
| B. Rol docente | Sencillo y didáctico           | Analogías de la vida real (cajas con etiquetas)            | Estudiantes principiantes              |
| C. Rol senior  | Alto nivel técnico             | Código Java, tipos de datos, gestión de memoria Stack/Heap | Desarrolladores / Compañeros de equipo |

---

## Ejercicio 5: Descomposición

### Registro por Pasos vs. Pedido Único

- **Pedido único:** La IA generó una estructura genérica, simplificada y mezclada de inventario en una sola respuesta superficial.
- **Paso 1:** Entregó los 5 requisitos principales (Gestión de productos, control de stock, registro de entradas/salidas, alertas de stock mínimo y reportes).
- **Paso 2:** Diseñó el diagrama de clases (`Producto`, `Inventario`, `Movimiento`, `Proveedor`) detallando atributos y tipos de datos.
- **Paso 3:** Escribió el código modular y limpio para la clase `Producto.java`.
- **Paso 4:** Ofreció 3 mejoras concretas: validación de stock negativo en setters, implementación de patrón Builder e integración de identificador UUID.

--

## Ejercicio 6: Prompt estructurado y autocrítica

```text
<rol>Actúa como analista de pruebas de software.</rol>
<contexto>Login web con correo y contraseña. La cuenta se bloquea después de 3 intentos fallidos.</contexto>
<tarea>Piensa paso a paso qué puede fallar y escribe 6 casos de prueba.</tarea>
<formato>Tabla con las columnas: ID, escenario, datos de entrada, resultado esperado.</formato>

[Mensaje de Autocrítica enviado posteriormente en la misma sesión]:
Revisa tu tabla: ¿faltan casos límite como campos vacíos, correo sin @ o contraseña con espacios? Agrega los que falten e indica cuáles agregaste.
```

- [Bitacora de tecnicas avanzadas](prompts/BITACORA.md)
