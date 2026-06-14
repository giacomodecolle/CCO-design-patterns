---
config:
      theme: redux
---
flowchart BT
A{event 1}
B{city 1}
C{city part 1}
D{month 1}
E{multi-month temporal interval 1}
F{time of day 1}
G[multi-month temporal event ont00000329]
H[spring 2004]
I[one dimensional temporal region BFO:0000038]
J[May 2004]
K[time of day ont00000223]
L[May 17th at 1:38pm EDT]
A -- occurs at --> B
A -- occurs at --> C
B -- has continuant part --> C
E -- rdf:type --> G
E -- rdf:label --> H
D -- rdf:type --> I
D -- rdf:label --> J
F -- rdf:type --> K
F -- rdf:label --> L