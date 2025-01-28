```mermaid

%Shows how to connect the Quality 'Weight' to an Agent 
graph BT
   %% Frank and 'weight 1' and are instances  
    A{Frank} --->|rdf:type| L[Agent<br>ont00001262]
    B{weight 1}--->|rdf:type| M[Weight<br>ont00000633]

    M --->|subClassOf| N[Quality<br>BFO_0000019 ]
    X@{ shape: text, label: "80 kg" }

    B -.-> X
    A --->|bearer of BFO_0000196| B


%% This section specifies the formatting of the links and nodes in the mermaid diagram 
%% mermaid comment: Changing the color of a link is on order of links created, in this instance 4 refers to the link between F{weight}-.->X (the 4th one to be created) 
 
    linkStyle 3 stroke:#FF0000

    classDef yellow fill:#ffe680,color:black
    classDef purple fill:#dbc9ef,color:black
    class A,B purple
    class L,M,N yellow
    
```