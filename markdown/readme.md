[Volver a sección principal](https://github.com/FrancoLCantero/cheatsheets/tree/main)

# **Apuntes de Markdown**

## **1. Introducción a Markdown**
Markdown es un lenguaje de marcado ligero que permite formatear texto de manera sencilla, usando caracteres de texto plano.
Fue creado por John Gruber y Aaron Swartz en 2004 con el objetivo de ser legible tanto en texto plano como en formato HTML.
Es ampliamente utilizado para documentación, blogs y README de proyectos.

### Características principales de Markdown:
1. **Simplicidad:** Markdown es fácil de aprender y usar, con una sintaxis sencilla para dar formato a texto.
2. **Conversión a HTML:** Se puede convertir fácilmente a HTML, lo que permite su uso en blogs, documentación, y más.
3. **Compatibilidad:** Muchos sistemas de gestión de contenidos, foros y plataformas de desarrollo, como GitHub, soportan Markdown.

## **2. Sintaxis Básica**

### **2.1. Encabezados**
Se crean usando el símbolo `#`. Puedes usar de uno a seis `#` para definir el nivel del encabezado:

```markdown
# Encabezado Nivel 1
## Encabezado Nivel 2
### Encabezado Nivel 3
#### Encabezado Nivel 4
##### Encabezado Nivel 5
###### Encabezado Nivel 6
```

### **2.2. Estilos de Texto**

| *MarkDown*                            | *Nombre*         | *Ejemplo*                                | *Uso*                                                                 |
| ------------------------------------- | ---------------- | ---------------------------------------- | --------------------------------------------------------------------- |
| `**Negrita**`                         | Negrita          | **Negrita**                              | Para resaltar texto importante.                                       |
| `*Cursiva*`                           | Cursiva          | *Cursiva*                                | Para enfatizar palabras o frases.                                     |
| `_Itálica_`                           | Itálica          | _Itálica_                                | Alternativa para enfatizar, similar a cursiva.                        |
| `__Subrayado__`                       | Subrayado        | __Subrayado__                            | Para subrayar texto (usualmente no es estándar en Markdown puro).     |
| `~~Tachado~~`                         | Tachado          | ~~Tachado~~                              | Para indicar texto que debe ser ignorado o eliminado.                 |
| `> Cita`                              | Cita             | > Esto es una cita                       | Para citar o resaltar texto citado.                                   |
| `` `Código` ``                        | Código en línea  | `` `print("Hola")` ``                    | Para resaltar fragmentos de código en línea.                          |
| \`\`\`                                | Bloque de código | \`\`\` python \n print("Hola") \n \`\`\` | Para bloques de código multilínea, con o sin especificar el lenguaje. |
| `---`                                 | Separador        | ---                                      | Para crear una línea horizontal separadora.                           |

### **2.3. Listas**

- **Listas Desordenadas:** Usa `-`, `*` o `+` como viñetas.
- **Listas Ordenadas:** Usa números seguidos de un punto.

```markdown
- Elemento 1
- Elemento 2

1. Elemento 1
2. Elemento 2
```

### **2.4. Enlaces**

| **[[MarkDown - Definición\|MarkDown]]**     | **Nombre**        | **Ejemplo**                                                        | **Uso**                                         |
| ------------------------------------------- | ----------------- | ------------------------------------------------------------------ | ----------------------------------------------- |
| `[[Nota Interna]]`                          | Enlace interno    | `[[Mi Nota]]`                                                      | Para enlazar a otras notas dentro de Obsidian.  |
| `[Texto del enlace](URL)`                   | Enlace externo    | `[Documentación Markdown](https://markdown.es/sintaxis-markdown/)` | Para enlazar a páginas web o recursos externos. |
| `![Texto alternativo](URL)`                 | Imagen            | `![Logo de Markdown](https://example.com/logo.jpg)`                | Para insertar imágenes con texto alternativo.   |
| `[Texto del enlace](URL "Título opcional")` | Enlace con título | `[Guía Markdown](https://example.com "Guía completa de Markdown")` | Añadir un título emergente a un enlace.         |

### **2.5. Imágenes**

Para insertar imágenes:

```markdown
![Texto alternativo](url-de-la-imagen)
```

Ejemplo:

```markdown
![Logo de Markdown](https://markdown-here.com/img/icon256.png)
```

### **2.6. Citas**

Para agregar citas usa el símbolo `>`:

```markdown
> Esto es una cita.
```

### **2.7. Código**

- **Código en Línea:** Usa `` ` ``.

```markdown
`Este es un código en línea.`
```

- **Bloques de Código:** Usa tres tildes invertidas o tres backticks ```` ``` ````. Puedes especificar el lenguaje para resaltar sintaxis.

```markdown
```javascript
console.log("Hola, Markdown!");
```
```

## **3. Tablas**
Puedes crear tablas con el siguiente formato:

```markdown
| Encabezado 1 | Encabezado 2 |
|--------------|--------------|
| Celda 1      | Celda 2      |
| Celda 3      | Celda 4      |
```

Resultado:

| Encabezado 1 | Encabezado 2 |
|--------------|--------------|
| Celda 1      | Celda 2      |
| Celda 3      | Celda 4      |

### 2.8 **GitHub**

| Funcionalidad              | Código en [[MarkDown - Definición\|Markdown]] | Ejemplo                  |
| -------------------------- | --------------------------------------------- | ------------------------ |
| Emojis                     | `:smiley:` `:+1:`                             | :smiley: :+1:            |
| Notificar a otros usuarios | `@NombreDeUsuarioEnGitHub`                    | @NombreDeUsuarioEnGitHub |

### 2.9 **Obsidian**

> [!NOTE] Title
> Contents

> [!WARNING] Title
> Contents

> [!INFO] Title
> Contents

> [!TIP] Title
> Contents


## **4. Otros Elementos Útiles**

### **4.1. Separadores**

Para añadir una línea horizontal:

```markdown
---
```

### **4.2. Checklists**

Para crear listas con casillas de verificación:

```markdown
- [x] Tarea completada
- [ ] Tarea pendiente
```

### **4.3. Escapar Caracteres**

Usa la barra invertida `\` para escapar caracteres especiales:

```markdown
\*Este texto no estará en cursiva\*
```

## **5. Consejos para Markdown**

- Mantén el texto limpio y bien organizado.
- Usa títulos y listas para mejorar la legibilidad.
- Familiarízate con las herramientas que soportan Markdown (por ejemplo, VS Code, GitHub, Notion).

## **6. Herramientas y Recursos**

### **6.1. Visualizadores de Markdown**
- [Markdown Here](https://markdown-here.com/)
- [Dillinger](https://dillinger.io/)

### **6.2. Convertidores**
- [Pandoc](https://pandoc.org/) (para convertir entre Markdown y otros formatos como PDF o HTML).

[Volver a sección principal](https://github.com/FrancoLCantero/cheatsheets/tree/main)

---
Last Edited on: 12/12/2024

