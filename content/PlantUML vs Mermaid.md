---
tags:
  - coding
  - modeling
created: 2023-07-08T11:37-05:00
updated: 2023-07-20T13:41-05:00
---
**Older & more developed vs Newer & more streamlined**

[[PlantUML]] and [[Mermaid]] are both [[Diagrams as Code]]  solutions aimed at providing ways to create UML (mostly) diagrams without taking your hands off the keyboard. They cover a *lot* of the same ground as each other, and have only really a few points of distinction separating them. Choosing between them comes down to:

1. Any specific diagrams you need that aren’t supported by both
2. Your desired deployment environment
3. Syntactic preferences 

# Diagram Coverage

| Graph Type | PlantUML | Mermaid |
| --- | --- | --- |
| Class Diagrams [[Class Diagrams]]  | ✅ | ✅ |
| State Diagrams [[State Diagrams]]  | ✅ | ✅ |
| Entity-Relationship Model [[Entity-Relationship Model]]  | ✅ | ✅ |
| Flow Charts [[Flow Charts]]  | ✅ | ✅ |
| Gantt Charts [[Gantt Charts]]  | ✅ | ✅ |
| Pie Chart | ❌ | ✅ |
| Sequence Diagrams [[Sequence Diagrams]]  | ✅ | ✅ |
| Timing Diagram | ✅ | ❌ |
| Use Case Diagrams [[Use Case Diagrams]]  | ✅ | ❌ |
| Activity Diagrams [[Activity Diagrams]]  | ✅ | ❌ |
| JSON [[JSON]] Views | ✅ | ❌ |
| Requirements Diagram [[Requirements Diagram]]  | ❌ | ✅ |

---

## Source


# Deployment

Both PlantUML and Mermaid offer online diagram generators. Currently Mermaid's  is by far and away better than PlantUMLs by any metric.

[Online FlowChart & Diagrams Editor - Mermaid Live Editor](https://mermaid.live/)

[PlantUML Web Server](https://www.plantuml.com/plantuml/uml)

A major difference between the two platforms is that PlantUML expects to be installed *locally* and used to create diagrams that are saved *locally*, whereas Mermaid expects you’ll be using it in the browser to render graphs to a webpage. 

Installing **PlantUML** involves downloading & installing:

1. Java
2. Graphviz (which handles layouts) 
3. PlantUML

Interestingly it looks like PlantUML is *also* available [via NPM](https://www.npmjs.com/package/plantuml) - it’s just not officially supported.

**Mermaid’s** intended application is via inclusion as a <script> tag using a CDN, or through local install using NPM... both of which are much easier. You could simply copy/paste the below into a text file on your computer, save it with a ‘.html’ suffix, then open it in your browser to see your diagram.

```html
<html>
        <script src="https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
        <body>
            Here is a mermaid diagram:
            <div class="mermaid">
                graph TD 
                A[Client] --> B[Load Balancer] 
                B --> C[Server01] 
                B --> D[Server02]
            </div>
            <script>
                mermaid.initialize({ startOnLoad: true });
            </script>
    </body>
</html>
```

Both Mermaid and PlantUML enjoy some level of native application support. You can utilize them to create diagrams with minimal configuration (and sometimes *no configuration*) in the following environments.

### Mermaid Application Support

Productivity Apps:

Notion

Confluence*

Code Versioning Tools:

GitLab

GitHub - pledged support soon

Code Editors:

VS Code*

Atom*

Sublime*

VIM*

Generated Documentation:

Sphinx*

Typedoc*

### PlantUML Application Support

Productivity Apps:

Confluence*

Word*

Code Versioning Tools:

GitBucket*

GitLab

Code Editors:

VS Code*

Atom*

Eclipse*

IntelliJ IDEA*

Generated Documentation:

Swagger API*

Typedoc*

Asterisked items (*) require plugins and/or configuration. Also both lists are partial. See [Mermaid’s list](https://mermaid-js.github.io/mermaid/#/./integrations) and [PlantUMLs list](https://plantuml.com/running).

# Syntax Comparison

They aren’t grossly different, but on the whole PlantUML is more *descriptive*, whereas Mermaid is more graphically *representative*. Here are a couple of bite-sized examples of the input syntax and output graphics for your consideration. These were created using the online tools found on each of their respective home pages ([Mermaid.live](https://mermaid.live/) and [http://www.plantuml.com/plantuml/uml](http://www.plantuml.com/plantuml/uml)).

## Class Diagrams

### PlantUML

### Mermaid

### Related Notes
- [[Mermaid]] 
- [[PlantUML]] 
- [[UML]]