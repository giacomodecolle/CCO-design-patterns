```mermaid
graph BT
    A{Measurement of Pencil Mass 1} --->|rdf:type| B[Measurement Information Content Entity
    ont00001163]
    A --->|generically depends on BFO_0000084| C{Balance Display 1}
    C --->|rdf:type| D[Information Bearing Entity ont00000253]
    C --->|uses measurement unit ont00001863| E{Gram Measurement Unit}
    E --->|rdf:type| F[Measurement Unit of Mass ont00000239]
    C --->|has decimal value ont00001769| G[8.4]

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#ffffff
    class B,D,F yellow
    class A,C,E purple
    class G white


