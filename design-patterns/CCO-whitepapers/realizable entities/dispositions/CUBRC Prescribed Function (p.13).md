graph BT
        A{grenade 1} --->|bearer of BFO_0000196| B{explosive artifact 
        function 1}
        A --->|prescribed by ont00001920| C{artifact model 1}
        A --->|rdf:type| D[Grenade
        ont00000310]
        C --->|rdf:type| E[Artifact Model
        ont00001045]
        B --->|rdf:type| F[Explosive Artifact Function
        ont00000841]
        C -.->|rdfs:label| G[Arges Type HG 84]

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#ffffff
    class D,E,F yellow
    class A,B,C purple
    class G white
