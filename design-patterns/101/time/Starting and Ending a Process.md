```mermaid

graph BT
    A{Flight Take-Off} --->|rdf:type| B[Process Beginning ont00000197]
    A --->|temporal part of BFO_0000139| C{Flight from Tokyo to Paris}
    C --->|rdf:type| E[Process 
    BFO_0000015]
    D{Flight Touch-Down}--->|rdf:type| F[Process Ending ont00000083]
    D--->|temporal part of BFO_0000139| C

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    class B,E,F yellow
    class A,C,D purple

