graph BT
        A{agent 1} --->|agent in ont00001787| B{act of ownership 1}
        B --->|has participant BFO_0000057| C{vehicle 1}
        C --->|bearer of BFO_0000196| D{financial value of property 1}
        D --->|is measured by ont00001904| E{measurement information content entity 1}
        E --->|generically depends on BFO_0000084| F{information bearing entity 1}
        F --->|has integer value ont00001773| G[19995]
        F --->|uses measurement unit ont00001863| H{United States Dollar}
        D --->|rdf:type| I[Financial Value of Property
        ont00001073]
        H --->|rdf:type| J[Measurement Unit of Currency
        ont00000518]
        F --->|rdf:type| K[Information Bearing Entity
        ont00000253]
        E --->|rdf:type| L[Measurement Information Content Entity
        ont00001163]
        C --->|rdf:type| M[Vehicle ont00000713]
        B --->|rdf:type| N[Act of Ownership
        ont00001336]
        A --->|rdf:type| O[Agent
        ont00001017]

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#ffffff
    class I,J,K,L,M,N,O yellow
    class A,B,C,D,E,F,H purple
    class G white
