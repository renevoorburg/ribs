# RIBS - RDA Improved By Simplification

Goal of RIBS is to make it easier for humans to work with the RDA (Resource Description and Access) metadata standard in an RDF based context.

This is done by

* Getting rid of all elements (properties) that are unnecessary when refered object entities are properly typed. This allows RIBS to get rid of a substantial set of elements that explicitly refer to a subclass of `<http://rdaregistry.info/Elements/c/C10002>` (`"Agent"`) . They can be replaced by a generic super property, keeping the full RDA semantics, when the entities are properly typed. For example, RDA elements `"is moderator person of"` (`rdfs:domain "Person"`) and `"is moderator family of"` (`rdfs:domain "Family"`), etcetera, can be replaced with the generic `"is moderator of"` (`rdfs:domain "Agent"`) .
* Adding some versatile, generic elements like `related` or `subjectOf`.
* Getting rid of all cryptical properties and classes like `rdac:C10008` and `rdae:P20319` and replacing them by something more human friendly like `ribs:Family` and `ribs:aggregates`.
* Aggregating all RDF definitions into one resource, allowing the use of a single namespace prefix '`ribs:`' in stead of requiring the extended set of namespace prefixes like `rdac:`, `rdae:`, `rdaw:`, `rdam:`, *etcetera*, that are needed for RDA. 



A work in progress.