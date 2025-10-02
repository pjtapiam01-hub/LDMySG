---
sidebar_position: 0
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';


# Introducción a los LLMM

## **¿Qué es Lenguaje de Marcas?** 

Un **lenguaje de marcas** (también conocido como *markup language*) es un lenguaje diseñado para **describir, estructurar o etiquetar información** dentro de un documento. A diferencia de los lenguajes de programación tradicionales, los lenguajes de marcas **no incluyen estructuras de control** como bucles o condicionales, sino que se enfocan en representar datos de forma jerárquica y comprensible tanto para humanos como para máquinas.

Un lenguaje de marcas utiliza **etiquetas (tags)** para identificar las distintas partes del contenido. Por ejemplo:

```xml
// highlight-next-line
<libro>
     <titulo> El nombre del viento</titulo> 
     <autor> El camino de los Reyes</autor>
     <coleccion> 
        <nombre> El archivo de las tormentas </nombre>
        <numero> 1</numero>
     <coleccion>
  // highlight-next-line
</libro>
```

Este fragmento describe un libro usando una estructura jerárquica de etiquetas.

<div style={{ display: 'flex', justifyContent: 'center' }}>
  <img src="/img/llmm/UT0/Diagrama Libro.png" alt="Estructura jerárquica XML" title="Estructura jerárquica XML" />
</div>

---

## **¿Para qué se usan los lenguajes de marcas?**

Los lenguajes de marcas se aplican en diversos contextos tecnológicos. Algunos de sus principales usos son:

* **Desarrollo web**: HTML estructura las páginas, CSS las presenta y JavaScript las hace interactivas. XML puede servir de base de datos.
* **Intercambio de información entre sistemas**: XML y JSON son formatos comunes para APIs.
* **Documentación técnica**: DocBook o LaTeX.
* **Edición y publicación digital**: EPUB (basado en HTML y XML).
* **Aplicaciones empresariales**: Intercambio de datos con XML (facturas electrónicas, pedidos, etc.).

---

## **Características de los lenguajes de marcas**

* **Jerárquicos**: Organizan la información en forma de árbol.
* **Auto-descriptivos**: Las etiquetas explican el contenido que encapsulan.
* **Legibles**: Están pensados para ser comprensibles tanto por personas como por sistemas.
* **Separación de contenido y presentación**: Especialmente útil en el desarrollo web.
* **Extensibles**: Algunos lenguajes permiten crear nuevas etiquetas según las necesidades del usuario (como XML).

---

## **Tipos de lenguajes de marcas**
Existe una gran variedad de Lenguajes de Marcas, dependiendo de sus características podemos realizar diferentes clasificaciones entre ellos.Una clasificación simplificada es la que los divide en dos conjuntos principales de lenguakes de marcas:

### Lenguajes descriptivos o semánticos

Este tipo de lenguajes están orientados a describir la estructura de los datos que contienen. Los ejemplos más comunes de este tipo de lenguajes son los siguientes:

* **XML (eXtensible Markup Language)**: Es el estándar más conocido para el intercambio de datos estructurados entre aplicaciones.
* **JSON (JavaScript Object Notation)** Es un formato de intercambio de datos ligero y fácil de leer tanto para humanos como para máquinas. Se utiliza para almacenar y transmitir información estructurada, especialmente en aplicaciones web y APIs.

:::note Ejemplos
A continuación se presenta la información de un libro en diferentes lenguajes.
<Tabs>
    <TabItem value="XML" label="XML">
      ```xml
        <libro>
          <titulo> El camino de los Reyes </titulo> 
          <autor> Brandon Sanderson </autor>
          <coleccion> 
              <nombre> El archivo de las tormentas </nombre>
              <numero> 1 </numero>
          <coleccion>
        </libro>
      ```
    </TabItem>
    <TabItem value="json" label="JSON">
     ```json
      { 
        "libro": {
          "titulo": "El camino de los Reyes",
          "autor": "Brandon Sanderson",
          "coleccion": {
            "nombre": "El archivo de las tormentas",
            "numero": "1"
          }
        }
      }
     ```
    </TabItem>
 </Tabs>
:::

### Lenguajes procedimentales y de presentación 

Este tipo de lenguajes están orientados a especificar cómo debe representarse la información. Los ejemplos más comunes de este tipo de lenguajes son los siguientes:

* **HTML (HyperText Markup Language)**: Usado para estructurar páginas web.
* **MarkDown**: Es un lenguaje de marcado ligero que sirve para dar formato a texto de forma sencilla, utilizando una sintaxis mínima y fácil de recordar.

:::note Ejemplos
A continuación se representa el siguinete formato en HTML y MarkDown.
<div style={{ display: 'flex', justifyContent: 'center' }}>
  <img src="/img/llmm/UT0/Ejemplo formato.jpg" alt="Ejemplo Formato" title="Ejemplo Formato" />
</div>
<Tabs>
    <TabItem value="HTML" label="HTML">
      ```HTNML
          <h1>Hola mundo</h1>

          <p>Este es un <strong>texto en negrita</strong> y este en <em>cursiva</em>.</p>

          <ul>
            <li>Elemento 1</li>
            <li>Elemento 2</li>
            <li>Elemento 3</li>
          </ul>
      ```
    </TabItem>
    <TabItem value="MarkDown" label="MarkDown">
     ```MarkDown
          # Hola mundo

          Este es un **texto en negrita** y este en *cursiva*.

          - Elemento 1
          - Elemento 2
          - Elemento 3
     ```
    </TabItem>
 </Tabs>
:::

---
:::warning
  Existen una gran cantidad de lenguajes de marcas, los que hemos vistos son ejemplos de aquellos que encontraremos más a menudo.
:::
---

## **¿Qué vamos a parender en este módulo?**

Los lenguajes de marcas son **fundamentales en el desarrollo de aplicaciones web** y en el **intercambio de información estructurada**. A lo largo del módulo se explorarán distintos lenguajes. Nos centraremos principalmente en dos:

* Por una parte estudiaremos el lenguaje HTML y las tecnologías que lo acompañan para el desarrollo de páginas WEB como son (CSS y Java Script).
<div style={{ display: 'flex', justifyContent: 'center', height: '250px'  }}>
  <img src="/img/llmm/UT0/Tecnologias_HTML.png" alt="Tecnologías HTML" title="Tecnologías HTML" />
</div>
<p></p>
 
* Por otro lado estudiaremos XML y los lenguajes que permiten su validación (DTD y SCHEMA), su transformación (XSLT) y su consulta (XPath y XQuery)
<div style={{ display: 'flex', justifyContent: 'center' }}>
  <img src="/img/llmm/UT0/Tecnologias_XML.png" alt="Tecnologías XML" title="Tecnologías XML" />
</div>
---

## **¿Qué herramientas vamos a usar?**
Para trabajar los contenidos de este módulo emplearemos uno de los editores de texto más extendidos entre la comunidad de desarolladores como es [**VSCode**](https://code.visualstudio.com/).  

<div style={{ display: 'flex', justifyContent: 'center', padding:'20px' }}>
  <img src="/img/llmm/UT0/VSCode.jpg" alt="VSCode" title="VSCode" />
</div>

Además, emplearemos los navegadores mas comunes...

<div style={{ display: 'flex', justifyContent: 'center' }}>
  <img src="/img/llmm/UT0/Navegadores.png" alt="Navegadores" title="Navegadores" />
</div>
:::warning
  VSCode no es un IDE y por lo tanto, aunque puede adaptarse a diferentes lenguajes de marcas y lenguajes de programación, no es el más indicado para el desarrollo de aplicaciones en lenguajes más complejos como Java.
:::


---

