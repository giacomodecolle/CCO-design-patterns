flowchart BT
    B{"June 24th, 2025 5pm-7:30pm PST"} -- rdf:type --> E["Temporal Region BFO_0000008"]
    B -- isTemporalRegionOf_ont00001874 --> A{"Marriage of William and Jennifer"}
    A -- rdf:type --> D["Process BFO_0000015"]

     B:::IndividualColor
     E:::ClassColor
     A:::IndividualColor
     D:::ClassColor
    classDef IndividualColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#E1BEE7
    classDef ClassColor stroke-width:1px, stroke-dasharray: 0, stroke:#AA00FF, fill:#FFF9C4


    subgraph Legend
    AA{Individual}
    BB[Class]
    CC[data]
    BB --> |relation| CC
    DD[This pattern demonstrates the usage of the inverse of the occupiesTemporalRegion object property, which is isTemporalRegionOf.] 

     
classDef yellow fill:#ffe680
classDef purple fill:#dbc9ef
classDef white fill:#ffffff
class BB yellow
class AA purple
class CC white
end