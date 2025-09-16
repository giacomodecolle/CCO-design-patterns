mermaid

flowchart TD
    A{"Measurement of tree length"} -- "rdf:type" --> B["Measurement Information Content Entity_00001163"]
    A -- generically_depends_on_0000084 --> C{"Piece_of_paper"}
    C -- "rdf:type" --> D["Information Bearing Entity_00000253"]
    C -- uses measurement unit_00001863--> E{"Meters Measurement Unit"}
    C -- has decimal value_00001769 --> F["10.2"]
    E -- "rdf.type" --> G["measurement unit_00000120"]
    I{length} --> |rdf:type| H["Entity_0000001"]
    A --> |is measurement of_00001966| I

    subgraph Legend
    AA{Individual}
    BB[Class]
    CC[data]
    BB --> |relation| CC
    DD[This pattern uses length as examples but can be reused for any other entity such as processes, qualities, people, etc.] 

     
classDef yellow fill:#ffe680
classDef purple fill:#dbc9ef
classDef white fill:#ffffff
class BB,B,D,G,H yellow
class AA,A,C,E,I purple
class CC,F white
end
