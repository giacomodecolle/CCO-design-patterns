flowchart BT
    A@{ label: "<font color=\"#000000\">Facility 1</font>" } -- LocatedIn<br>BFO:0000171 --> B@{ label: "<font color=\"#000000\">City 1</font>" }
    B -- LocatedIn<br>BFO:0000171 --> C@{ label: "<font color=\"#000000\">State 1</font>" }
    A -- rdf:type --> D@{ label: "<span style=\"color:black\"><b>Facility<br>ont00000192</b></span><br>" }
    B -- rdf:type --> E@{ label: "<span style=\"color:black\"><b>Site<br>BFO_0000029</b></span><br>" }
    C -- rdf:type --> E
    A -. rdfs:label .-> F["Empire State Building"]
    B -. rdfs:label .-> G["New York City"]
    C -. rdfs:label .-> H["New York State"]

    subgraph Legend
    AA{Individual}
    BB[Class]
    CC[data]
    AA --> |relation| CC
    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#ffffff
    class BB yellow
    class AA purple
    class CC white
    end

    A@{ shape: diam}
    B@{ shape: diam}
    C@{ shape: diam}
    D@{ shape: rect}
    E@{ shape: rect}
    F@{ shape: rect}
    G@{ shape: rect}
    H@{ shape: rect}
    A:::purple
    B:::purple
    C:::purple
    D:::yellow
    E:::yellow
    F:::white
    G:::white
    H:::white
    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#FFFFFF

    