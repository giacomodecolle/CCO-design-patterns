graph BT
    A{Hour-Long
    Temporal Region 1} -->|rdf:type| B[Temporal Region BFO_0000008]
    C{Beginning Moment
    of Hour 1} -->|first instant of BFO_0000221| A
    D{Ending Moment
    of Hour 1} -->|last instant of 
    BFO_0000223| A
    C -->|precedes 
    BFO_0000063| D
    C -->|rdf:type| E[Temporal Instant BFO_0000203]
    D -->|rdf:type| E

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    class B,E yellow
    class A,C,D purple