# Tarea: Mi prompt profesional

## Funcionalidad elegida
Sistema para registrar y calcular el promedio de notas de estudiantes, mostrando si aprobaron o reprobaron.

---



## Versión 1: prompt básico

```text
Hazme un programa para notas.
```

**Qué cambié:** Solo pedí algo muy general sin dar detalles.

**Por qué:** No pensé en qué lenguaje, qué datos ni qué resultado necesitaba.

**Qué mejoró:** La respuesta fue corta y muy genérica; no sabía si quería texto, una tabla o código.

---
## Versión 2

```text
Crea un programa en Java para guardar notas de estudiantes y calcular el promedio. Dime si aprueban o no.
```

**Qué cambié:**  Agregué el lenguaje y el objetivo principal.

**Por qué:** La versión 1 era tan vaga que la IA podía dar cualquier cosa.

**Qué mejoró:** Ahora sí dio código en Java, pide los datos, calcula el promedio y muestra el resultado. Pero aún faltan cosas: no valida que las notas estén entre 0 y 20, no separa el código en dos clases y usó 10.5 como nota de aprobación en lugar de 11.

---

## Versión 3: prompt final

```text
Actúa como desarrollador de software. Escribe un programa en Java de consola que haga lo siguiente:

- Pide el nombre del estudiante y tres notas (cada una entre 0 y 20).
- Valida que ninguna nota sea menor a 0 ni mayor a 20; si lo es, pide ingresarla de nuevo.
- Calcula el promedio de las tres notas.
- Si el promedio es 11 o más → muestra "Aprobado". Si es menor → "Reprobado".
- Organiza el código en dos clases: Estudiante y Principal.
- No uses librerías externas.
- Al final del código, explica brevemente cómo funciona.
```
**Qué cambié:**  Agregué todo: rol, instrucción clara, cada paso, rango de notas, nota de aprobación exacta, organización por clases, restricción y explicación final.

**Por qué:** Las versiones anteriores dejaban muchas cosas a la imaginación y el resultado no era exactamente lo que quería.

**Qué mejoró:** : El código salió completo, validando cada nota, con las dos clases separadas, la nota de corte en 11, sin librerías externas y con la explicación incluida. Cumple todo lo que pedí.

## Componentes del prompt final

| Componente | Qué dice en mi prompt |
|---|---|
| Rol | Actúa como desarrollador de software |
| Instrucción | Escribe un programa en Java de consola para gestionar notas |
| Contexto | Pide nombre y tres notas, valida rango, calcula promedio, muestra estado |
| Ejemplos / Criterios | ≥ 11 = Aprobado; < 11 = Reprobado; notas entre 0 y 20 |
| Formato | Dos clases: Estudiante y Principal; explica al final |
| Restricción | No uses librerías externas |

## Evaluación del resultado

| Qué revisar | Cumple (Sí / No) |
|---|---|
| ¿Está en Java y funciona en consola? | Sí |
| ¿Pide nombre y tres notas? | Sí |
| ¿Valida que las notas estén entre 0 y 20? | Sí |
| ¿Calcula el promedio y muestra el estado? | Sí |
| ¿Está organizado en dos clases? | Sí |


## Errores que evité

| Error frecuente | Cómo lo evité |
|---|---|
| Ser demasiado general | En la versión 1 solo dije "hazme un programa para notas". La IA no supo si era app, página o código. En la final lo especifiqué todo detalladamente |
| Asumir información no proporcionada | En la versión 2 la IA usó 10.5 como nota de aprobación porque no se lo indiqué. En la final lo escribí claramente: ≥ 11 = Aprobado |