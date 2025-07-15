graph BT
   %% Frank and 'weight 1' and are instances  
    A{Frank} --->|rdf:type| L[Person<br>ont00001262]
    B{weight 1}--->|rdf:type| M[Weight<br>ont00000633]

    M --->|subClassOf| N[Quality<br>BFO_0000019 ]
    X@{ shape: text, label: "80 kg" }

    B -.-> X
    A --->|bearer of BFO_0000196| B

    linkStyle 3 stroke:#FF0000

    classDef yellow fill:#ffe680,color:black
    classDef purple fill:#dbc9ef,color:black
    class A,B purple
    class L,M,N yellow
