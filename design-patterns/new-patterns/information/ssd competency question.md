graph BT
B{Information 1} -->|rdf:type| E[Information Content Entity
ont00000958]
G[Process
BFO_0000015]

I{Solid State Drive 1} -->|rdf:type| C[Information Bearing Entity
ont00000253]
A{Monitor 1} -->|rdf:type| L[Instrument Display Panel
ont00000597]

B -->|generically depends on
BFO_0000084| I
B -->|generically depends on
BFO_0000084| A

B --> |participates in
BFO_0000056| M{Display of Information in Monitor 1}
M --> |rdf:type| G

I --> |participates in
BFO_0000056| M
A --> |participates in
BFO_0000056| M
A --> |participates in
BFO_0000056| N

N --> |concretizes
BFO_0000059| B

N --> |occurs in
BFO_0000066| A
M --> |occurs in
BFO_0000066| A

M --> |has process part
ont00001777| N{Process of Pixels Displaying Information 1}
N --> |rdf:type| G
B --> |participates in
BFO_0000059| N

classDef yellow fill:#ffe680
classDef purple fill:#dbc9ef
classDef white fill:#ffffff

class C,E,G,L,O yellow
class A,B,F,H,I,M,N purple
class D white
