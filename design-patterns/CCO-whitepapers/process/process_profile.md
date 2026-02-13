flowchart TB
    subgraph Legend
        A{Individual}
        B[Class]
        C[data]
        B --> |relation| C
    end
    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#ffffff
    class B yellow
    class A purple
    class C white

    PS[Watercraft<br>ont00000440]:::yellow
    AM[Act of Motion<br>ont00000357]:::yellow 
    PP[Process Profile<br>BFO 000314]:::yellow
    S[Speed<br>ont00000830]:::yellow -->|subclass of| PP
    TR[Temporal Region<br>BFO 000008]:::yellow

    %% Instances
    PS1{Patrol Ship 1}:::purple -->|rdf:type| PS
    AM1{Act of Motion 1}:::purple -->|rdf:type| AM
    S1{speed 1}:::purple -->|rdf:type| S
    TR1{Temporal Region 1}:::purple -->|rdf:type| TR

    %% Relationships
    PS1 -->|participates in| AM1
    AM1 -->|occurs on| TR1
    AM1 -->|has profile| S1
    
    %% Data values
    TR1 ---|tokenized by| D1[1.5 hours]:::white
    S1 ---|tokenized by| D2[12 knots]:::white
