graph BT
B{Information 1} -->|rdf:type| E[Information Content Entity<br>ont00000958]
G[Process<br>BFO_0000015]

I{Solid State Drive 1} -->|rdf:type| C[Information Bearing Entity<br>ont00000253]
A{Monitor 1} -->|rdf:type| L[Instrument Display Panel<br>ont00000597]

B -->|generically depends on<br>BFO_0000084| I
B -->|generically depends on<br>BFO_0000084| A

B --> |participates in<br>BFO_0000056| M{Display of Information 1}
M --> |rdf:type| G

I --> |participates in<br>BFO_0000056| M
A --> |participates in<br>BFO_0000056| M

M --> |occurs at<br>ont00001918| N{Monitor Site 1}
N --> |rdf:type| O[Site<br>BFO_0000029]

A --> |located in<br>BFO_0000171| N

classDef yellow fill:#ffe680
classDef purple fill:#dbc9ef
classDef white fill:#ffffff

class C,E,G,L,O yellow
class A,B,F,H,I,M,N purple
class D white
