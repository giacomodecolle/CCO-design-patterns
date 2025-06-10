flowchart BT
    A{"William Stephens"} -- rdf:type --> F["Person
    ont00001262"]
    A -- bearerOf_BFO0000196 --> H{"Student Role"}
    H -- rdf:type --> C["Role 
    BFO0000023"]
    H -- hasOrganizationalContext_ont00001992 --> K{"University of Buffalo"}
    K -- rdf:type --> E["Organization 
    ont00001180"]

     A:::IndividualColor
     F:::ClassColor
     H:::IndividualColor
     C:::ClassColor
     K:::IndividualColor
     E:::ClassColor
    classDef IndividualColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#E1BEE7
    classDef DataColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#FFFFFF
    classDef ClassColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#FFF9C4


