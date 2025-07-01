This document contains general guidelines for the creation of design patterns (DP), especially in the context of the BFO and CCO communities. The intent of DPs as understood in this document are numerous: they act as documentation for the ontology, insofar as they show how the resources in the ontology can be correctly used. They also provide a reusable template that can be implemented in a system using ontologies, for example to guide instantiation or to write SPARQL queries that look for the presence of a certain structure. The current status of the guidelines discussed and adopted in the NCOR CCO working group are the following:

- The DP needs to have a clear and understandable legend.
- The DP needs to represent a graph structure of instances related to each other using relations from the ontology itself or from vocabularies such as RDF, OWL, etc. 
- The DP needs to clearly and unambiguously distinguish between classes, instances, relations and data. For example, by using different colors or shapes in the graph.
- Relations shall be represented as edges, while classes and instances are to be represented as nodes.
- The DP needs to label relations with the exact terminology taken by the ontology. If the ontology uses opaque IRIs, it is preferable to also add them.
- The DP needs to label classes with the exact terminology taken by the ontology. If the ontology uses opaque IRIs, it is preferable to also add them.
- The DP needs to have instances named with human-readable names (such as the ones that one would use in a human-readable label). For example, "John" can serve as the name of an instance of class "Person". 
- Instance names serve the purpose of providing an example of what in the world the class structure could be used to represent. Nevertheless, it is up to the author of the DP to make it clear that the structure can be reused for different cases as well.
- The class structure will be specified at the most general level. For example, a DP illustrating specific dependence will use the class "Specifically Dependent Continuant", and not the class "Quality" or "Role"
- All instances should have at least one parent class to make it clear where it fits in the BFO/CCO hierarchy.
