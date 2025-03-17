# 🐙  Formato avanzado

## Alertas

Las alertas son una extensión de Markdown basada en la sintaxis blockquote que puedes utilizar para resaltar información crítica. Se muestran con colores e iconos distintos para indicar la importancia del contenido.

> [!NOTE]
> Información útil que los usuarios deben saber, incluso cuando hojean el contenido.

> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.

> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.

> [!WARNING]
> Información urgente que necesita atención inmediata del usuario para evitar problemas.

> [!CAUTION]
> Informa sobre los riesgos o resultados negativos de determinadas acciones.

## Sección colapsada

Puedes contraer temporalmente secciones de tu Markdown creando una sección expandida que el lector puede elegir expandir. Por ejemplo, cuando desea incluir detalles técnicos en un comentario sobre un problema que pueden no ser relevantes o interesantes para todos los lectores, puede colocar esos detalles en una sección contraída.

Cualquier Markdown dentro del bloque `<details>` se contraerá hasta que el lector haga clic para expandir los detalles.

En el bloque `<details>`, utilice la etiqueta `<summary>` para que los lectores sepan qué hay dentro. La etiqueta aparece a la derecha de .

<details>

<summary>Consejos para secciones colapsadas</summary>

### Puedes agregar un encabezado

Puedes añadir texto dentro de una sección contraída.

También puedes añadir una imagen o un bloque de código.

```ruby
   "Hola Mundo"
```

</details>

## Diagramas de Mermaid (sirena)

Mermaid es una herramienta inspirada en Markdown que convierte texto en diagramas. Por ejemplo, Mermaid puede interpretar diagramas de flujo, diagramas de secuencia, gráficos circulares y más.

Para crear un diagrama de Mermaid, agregue la sintaxis de sirena dentro de un bloque de código independiente con el identificador de idioma Mermaid.

Por ejemplo, puede crear un diagrama de flujo especificando valores y flechas.

A continuación se muestra un diagrama de flujo simple:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

## Mapas

Puede utilizar la sintaxis GeoJSON o TopoJSON para crear mapas interactivos. Para crear un mapa, agregue GeoJSON o TopoJSON en un bloque de código protegido con el identificador de sintaxis geojson o topojson.

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              -90,
              35
            ],
            [
              -90,
              30
            ],
            [
              -85,
              30
            ],
            [
              -85,
              35
            ],
            [
              -90,
              35
            ]
          ]
        ]
      }
    }
  ]
}
```
