# Mallabot

Asistente de consola que responde preguntas en lenguaje natural sobre la malla curricular de
Ingeniería Informática y de Sistemas de la UNSAAC: código, créditos, área y semestre de cada
curso.

**Curso:** Pensamiento Computacional e Inteligencia Artificial — UNSAAC (2025-II)
**Lenguaje:** Python 3 (sin dependencias externas)

## Qué hace

El objetivo del proyecto era emular la experiencia de un asistente inteligente **sin usar
algoritmos de aprendizaje automático**: todo se resuelve con reglas.

**Detección de intención.** La pregunta se normaliza a minúsculas y se busca qué quiere saber
el usuario a partir de palabras clave: `código`, `créditos`, `área`, `semestre`. Cada
intención tiene su propia función de respuesta.

**Identificación del curso.** Se recorre el catálogo buscando qué nombre de curso aparece
dentro de la pregunta, de modo que el usuario puede escribir la pregunta como quiera
mientras nombre el curso.

**Catálogo.** 59 cursos de los diez semestres, con sus códigos, créditos, áreas y semestre
correspondiente, además de la consulta de todos los cursos de un semestre dado.

**Respuesta ante lo desconocido.** Si no se identifica ni el curso ni la intención, responde
con un mensaje de ayuda en lugar de fallar.

## Ejemplos

```
¿Cuál es el código de Cálculo I?
¿Cuántos créditos tiene Física I?
¿A qué área pertenece Programación I?
¿En qué semestre está Teoría de la Computación?
cursos por semestre
ayuda
```

Se sale con `salir`, `adios` o `chao`.

## Cómo ejecutarlo

```bash
python mallabot.py
```

Requiere Python 3. No hay que instalar nada.

## Autoría

Proyecto grupal de la asignatura, desarrollado por Pinto Armacta Higinio Jhunior,
Torres Cama Merelin Rubi, Checca Ccolqque Denis Yeison, Huaccanqui Velasquez Duvan Rodrigo,
Sicos Alcca Gabriel Omar y Challco Montufar Deivis Alexander.
