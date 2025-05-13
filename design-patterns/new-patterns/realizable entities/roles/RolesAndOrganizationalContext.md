flowchart BT
    A{"Person 1"} -- rdf:type --> F["Person
    ont00001262"]
    A -- hasValue --> G["xsd string"]
    A -- bearerOf_BFO0000196 --> H{"Role 1"}
    H -- rdf:type --> B["Some Role"]
    B -- rdf:type --> C["Role 
    BFO0000023"]
    H -- hasOrganiationalContext_ont00001992 --> K{"Organization 1"}
    K -- rdf:type --> D["Some Organization"]
    D -- rdf:type --> E["Organization 
    ont00001180"]

     A:::IndividualColor
     F:::ClassColor
     G:::DataColor
     H:::IndividualColor
     B:::ClassColor
     C:::ClassColor
     K:::IndividualColor
     D:::ClassColor
     E:::ClassColor
    classDef IndividualColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#E1BEE7
    classDef DataColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#FFFFFF
    classDef ClassColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#FFF9C4


