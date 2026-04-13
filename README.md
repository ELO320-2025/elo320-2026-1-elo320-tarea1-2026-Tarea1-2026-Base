# ELO320 Tarea1 2026

Nombre: XX YY

El texto a continuación ejemplifica cómo usar markdown (el formato que usamos en los read me). Por lo tanto, **se espera que lo borren antes de entregar, ya que acá debería ir el reporte**. Pueden usar páginas adicionales a esta, pero deben ser en formato markdown (.md) y deberán ser referenciados dentro de este archivo.
## Elementos básicos de Markdown

### Títulos

```markdown
# Título nivel 1
## Título nivel 2
### Título nivel 3
```

### Texto con énfasis

```markdown
**negrita**
*cursiva*
`código en línea`
```

### Listas

```markdown
- Elemento A
- Elemento B
  - Subelemento B1

1. Primer paso
2. Segundo paso
3. Tercer paso
```

### Bloques de código

Usa triple backtick y especifica el lenguaje para resaltado de sintaxis:

````markdown
```python
def saludo(nombre):
    print(f"Hola, {nombre}!")
```
````

Se verá así:

```python
def saludo(nombre):
    print(f"Hola, {nombre}!")
```

---

## Tablas

Las tablas se construyen con `|` para separar columnas y `---` para la fila de encabezado.

### Sintaxis

```markdown
| Columna 1 | Columna 2 | Columna 3 |
|-----------|-----------|-----------|
| Dato A    | Dato B    | Dato C    |
| Dato D    | Dato E    | Dato F    |
```

### Resultado

| Columna 1 | Columna 2 | Columna 3 |
|-----------|-----------|-----------|
| Dato A    | Dato B    | Dato C    |
| Dato D    | Dato E    | Dato F    |

### Alineación de columnas

Agrega `:` en la fila de separadores para controlar la alineación:

```markdown
| Izquierda | Centro  | Derecha |
|:----------|:-------:|--------:|
| texto     | texto   | texto   |
| 1234      | 1234    | 1234    |
```

| Izquierda | Centro  | Derecha |
|:----------|:-------:|--------:|
| texto     | texto   | texto   |
| 1234      | 1234    | 1234    |

### Ejemplo aplicado a la tarea

```markdown
| Archivo              | N° registros | Tiempo (s) | Memoria (MB) |
|:---------------------|-------------:|-----------:|-------------:|
| encuestas_50.txt     | 50           | 0.001      | 0.2          |
| encuestas_500.txt    | 500          | 0.008      | 1.4          |
| encuestas_5000.txt   | 5000         | 0.071      | 13.1         |
| encuestas_50000.txt  | 50000        | 0.693      | 128.7        |
```

| Archivo              | N° registros | Tiempo (s) | Memoria (MB) |
|:---------------------|-------------:|-----------:|-------------:|
| encuestas_50.txt     | 50           | 0.001      | 0.2          |
| encuestas_500.txt    | 500          | 0.008      | 1.4          |
| encuestas_5000.txt   | 5000         | 0.071      | 13.1         |
| encuestas_50000.txt  | 50000        | 0.693      | 128.7        |

---

## Imágenes

### Sintaxis básica

```markdown
![Texto alternativo](ruta/a/la/imagen.png)
```

- **Texto alternativo**: descripción breve de la imagen (para accesibilidad y si la imagen no carga).
- **Ruta**: puede ser relativa (dentro del repositorio) o una URL externa.

### Imagen local (recomendado)

Guarda tus imágenes en una carpeta `img/` o `assets/` dentro del proyecto:

```
Tarea1-2026-Base/
├── img/
│   ├── grafico_tiempo.png
│   └── grafico_memoria.png
├── README.md
└── ...
```

Luego en el README:

```markdown
![Gráfico de tiempo de ejecución](img/grafico_tiempo.png)
```

### Imagen con enlace

Puedes hacer que una imagen sea un enlace clicable:

```markdown
[![Texto alternativo](img/grafico_tiempo.png)](img/grafico_tiempo.png)
```

### Controlar el tamaño de una imagen

Markdown puro no soporta tamaño de imagen, pero puedes usar HTML:

```html
<img src="img/grafico_tiempo.png" alt="Gráfico de tiempo" width="500">
```

### Centrar una imagen

```html
<p align="center">
  <img src="img/grafico_tiempo.png" alt="Gráfico de tiempo" width="600">
</p>
```

---

## Consejos para la tarea

1. **Sé descriptivo**: explica qué hace tu código, no solo cómo ejecutarlo.
2. **Incluye resultados**: agrega tablas con los tiempos medidos para cada archivo de entrada.
3. **Agrega gráficos**: si generas gráficos de rendimiento, inclúyelos con `![...]()`.
4. **Usa bloques de código** para mostrar comandos de ejecución:
   ```markdown
   ```bash
   python mi_programa.py data/encuestas_500.txt
   ```
   ```

---

## Recursos adicionales

- [Guía oficial de Markdown en GitHub](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Editor online de Markdown](https://dillinger.io/)


## Declaración de uso de IA

En caso de haber utilizado algún modelo de lenguaje dentro del desarrollo de la tarea, no olvides que debes declararlo acá e incluir para qué se utilizaron, el/los modelos utilizados y los prompts.