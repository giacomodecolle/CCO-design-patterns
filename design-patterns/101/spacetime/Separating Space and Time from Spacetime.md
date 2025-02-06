graph BT
    A{Spatiotemporal Region Occupied by 10-11 AM Meeting} --->|rdf:type| B[Spatiotemporal Region BFO_0000011]
    A --->|temporally projects onto BFO_0000153| C{Temporal Extent of Spatiotemporal Region}
    A --->|spatially projects onto BFO_0000216| D{Spatial Extent of Spatiotemporal Region at Some Time During Hour}
    C --->|rdf:type| E[Temporal Region BFO_0000008]
    D --->|rdf:type| F[Spatial Region BFO_0000006]

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    class B,E,F yellow
    class A,C,D purple
