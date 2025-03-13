# Mermaid code for role

graph BT
    A{<span style="color:black"><b>Person 1</b><br><b>ont00001262</b></span><br>} --->|has role| B[<span style="color:black"><b>US President role 1</b></span><br><br>]
    B --->|rdf:type| C[<span style="color:black"><b>President of the United States role</b></span><br><br>]
    A --->|rdf:type| D[<span style="color:black"><b>Agent</b><br><b>ont00001017</b></span><br>]
    A --->|participates in<br>BFO:0000056| E{<span style="color:black"><b>Gain of Role</b><br><b>ont00001194</b></span><br>}
    E --->|rdf:type| F[<span style="color:black"><b>Gain of Type</b></span><br><br>]
    F --->|is subclass of| G[<span style="color:black"><b>Change</b><br><b>ont00000004</b></span><br>]
    E --->|occurs on| H{<span style="color:black"><b>Temporal Interval 1</b></span><br><br>}
    H --->|rdf:type| I[<span style="color:black"><b>Temporal Interval</b><br><b>BFO:0000202</b></span><br>]
    A-.-> J[<span style="color:white"><b>Barrack Obama</b></span>]
    H-.-> K[<span style="color:white"><b>20 January 2009</b></span>]

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    class C,D,F,G,I yellow
    class A,B,E,H purple
