flowchart BT
    D{John Doe}
    D -->|rdf:type| F[Person ont00001262]
    E{Doctor role 1} --> |inheres in BFO_0000197| D
    E --> |rdf:type| G[Occupation Role ont00000984]
    E --> |has organizational context ont00001992| H{United Health System}
    H --> |rdf:type| I[Organization ont00001180]
    
    
    subgraph Legend
    A{Individual}
    B[Class]
    C[data]
    B --> |relation| C
classDef yellow fill:#ffe680
classDef purple fill:#dbc9ef
classDef white fill:#ffffff
class B,F,G,I yellow
class A,D,E,H purple
class C white
end
