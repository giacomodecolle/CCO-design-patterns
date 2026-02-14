```mermaid

graph BT
        A{Person 1} --->|rdf:type| B[Agent 
        ont00001017]
        A -.->|rdfs:label| C[Barrack Obama]
        A --->|bearer of BFO_0000196| D{US President Role 1}
        D --->|rdf:type| E[role 
        BFO_0000023]
        A --->|participates in BFO_0000056| F{Stasis of Role 1}
        D --->|participates in BFO_0000056| F
        F --->|rdf:type| G[Stasis of Role
        ont00000824]
        F -->|occupies temporal region BFO_0000199| H{Temporal Interval 1}
        H --->|rdf:type| I[Temporal Interval
        BFO_0000202]
        H -.->|rdfs:label| J[8 years]

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#ffffff
    class B,E,G,I yellow
    class A,D,F,H purple
    class C,J white

