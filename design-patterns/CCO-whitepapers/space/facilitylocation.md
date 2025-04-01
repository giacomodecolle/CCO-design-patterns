flowchart BT
    A{"Facility 1"} -- |LocatedIn_BFO0000171| --> B{"City 1"}
    B -- |LocatedIn_BFO0000171| --> C{"State 1"}
    A -- |rdf:type| --> D["Facility 
    ont00001768"]
    B -- |rdf:type| --> E["Site BFO_0000029"]
    C -- |rdf:type| --> E
    A -- |rdfs:label| --> F["Empire State Building"]
    B -- |rdfs:label| --> G["New York City"]
    C -- |rdfs:label| --> H["New York State"]

    F@{ shape: rect}
    G@{ shape: rect}
    H@{ shape: rect}
    style A fill:#E1BEE7,stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style B fill:#E1BEE7,stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style C stroke:#AA00FF,fill:#E1BEE7,stroke-width:1px,stroke-dasharray: 0
    style D stroke:#AA00FF,fill:#FFE0B2,stroke-width:1px,stroke-dasharray: 0
    style E stroke:#AA00FF,fill:#FFE0B2,stroke-width:1px,stroke-dasharray: 0
    style F stroke:#AA00FF,stroke-width:1px,stroke-dasharray: 0
    style G stroke-width:1px,stroke-dasharray: 0,stroke:#AA00FF,fill:#FFFFFF
    style H stroke-width:1px,stroke-dasharray: 0,stroke:#AA00FF


