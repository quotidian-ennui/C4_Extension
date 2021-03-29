# C4_Extension
Coloring for https://github.com/plantuml-stdlib/C4-PlantUML

Using C4 diagrams in plantuml is great; but we're using it to denote systems that are actively under development and/or systems we want to retire. In effect a town plan of our internal product landscape and how they link to each other.

Essentially it just defines some new colours for `System_new`, `System_Legacy`, `System_PSO` because just having "System" is too boring.

```
System_New(bleeding_edge, "Buzzword Bingo", "Not on the edge\nTaking too much space.")
System_Legacy(old_skool, "Uncool", "Works but isn't cool")
System_PSO(duct_tape, "Random script", "It's a thing\nno one knows about")


old_skool ..> bleeding_edge: migrates
Rel(duct_tape, old_skool, "injects data into")
```
