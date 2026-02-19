```mermaid

flowchart TB
 subgraph Legend["Legend"]
        AA{"Individual"}
        BB["Class"]
        CC["data"]
        DD["This design pattern uses agents as agents in the act of targeting to show who is doing the targeting, but this is not needed to build the rest of the graph. The example is of a human being targeted but all material entities can be targeted."]
  end
    C{"Red Brigades"} -- Agent_in_ont00001787 --> B{"Targeting_Moro"}
    A{"Aldo Moro"} -- rdf:type --> D["Target_ont00000544"]
    A -- is object of
    ont00001936 --> B
    C -- rdf:type --> E["Agent_ont00001017"]
    D -- subclass_of --> g["Material_Entity BFO_0000040"]
    B -- rdf:type --> H["Act_of_Targeting_ont00000741"]
    BB -- relation --> CC

     AA:::purple
     BB:::yellow
     BB:::Class_22
     BB:::Class_23
     CC:::white
     C:::Class_03
     C:::Class_11
     B:::Class_08
     B:::Class_19
     B:::Class_21
     A:::Class_02
     A:::Class_10
     D:::Class_05
     D:::Class_12
     D:::Class_17
     E:::Class_06
     E:::Class_13
     E:::Class_18
     g:::Class_09
     H:::Class_20
    classDef Class_02 fill:#ffe680
    classDef Class_03 fill:#ffe680
    classDef Class_04 fill:#ffe680
    classDef Class_05 fill:#ffe680
    classDef Class_06 fill:#ffe680
    classDef Class_07 fill:#dbc9ef
    classDef Class_08 fill:#dbc9ef
    classDef Class_10 fill:#dbc9ef
    classDef Class_11 fill:#dbc9ef
    classDef Class_12 fill:#dbc9ef
    classDef Class_13 fill:#dbc9ef
    classDef Class_14 fill:#ffe680
    classDef Class_15 stroke:transparent
    classDef Class_16 fill:#ffe680
    classDef Class_17 fill:#ffe680
    classDef Class_18 fill:#ffe680
    classDef Class_19 fill:#ffe680
    classDef Class_09 fill:#ffe680
    classDef Class_20 fill:#ffe680
    classDef Class_21 fill:#dbc9ef
    classDef yellow fill:#ffe680,fill:#ffe680 
    classDef purple fill:#dbc9ef,fill:#dbc9ef 
    classDef white fill:#ffffff,fill:#ffffff
    classDef Class_22 fill:#dbc9ef
    classDef Class_23 fill:#ffe680
    style AA stroke:#E1BEE7
    style BB stroke:#E1BEE7
    style CC stroke:#E1BEE7
    style DD stroke:#E1BEE7
    style C stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style B stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style A stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style D stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style E stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style g stroke:#E1BEE7
    style H stroke:#E1BEE7
    style Legend stroke:#E1BEE7,fill:#E1BEE7
