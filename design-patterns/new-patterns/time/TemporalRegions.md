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


