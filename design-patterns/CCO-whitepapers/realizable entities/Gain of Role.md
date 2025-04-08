# Mermaid code for role

graph BT
    A{<span style="color:black"><b>Person 1</b><br><b></b></span><b} --->|bearer of<br>BFO:0000056 | B{<span style="color:black"><b>President Role 1</b></span><br>}
    B --->|rdf:type| C[<span style="color:black"><b>Role</b><b><br>BFO:000023</b></span><br>]
    A --->|rdf:type| D[<span style="color:black"><b>Agent</b><br><b>ont00001017</b></span><br>]
    A --->|participates in<br><b>BFO:0000056</b>| E{<span style="color:black"><b>Gain of Role 1</b></span><br>}
    E --->|rdf:type| F[<span style="color:black"><b>Gain of Role</b><b><br>ont00001194</b><br>]
    F --->|is subclass of| G[<span style="color:black"><b>Change</b><br><b>ont00000004</b></span><br>]
    E --->|occupies temporal region <br>ont0000199| H{<span style="color:black"><b>Temporal Interval 1</b></span><br>}
    H --->|rdf:type| I[<span style="color:black"><b>Temporal Interval</b><br><b>BFO:0000202</b></span><br>]
    

    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    class C,D,F,G,I yellow
    class A,B,E,H purple

