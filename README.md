# RIBS - RDA Improved By Simplification

Goal of RIBS is to make it easier for humans to work with the RDA (Resource Description and Access) metadata standard in an RDF based context.

This is done by

* Getting rid of all elements (properties) that are not needed when object entities are properly typed. This allow RIBS to get rid of a large set of elements that refer to a subclass of <http://rdaregistry.info/Elements/c/C10002> ("Agent") and have a super-property with a otherwise identical semantics.
* Getting rid of all cryptical properties and classes like `rdac:C10008` and `rdae:P20319` and replacing them by something more human friendly like `ribs:Family` and `ribs:aggregates`.
* Aggregating all definitions into one, allowing for the use of just one namespace prefix '`ribs:`' in stead of the many like `rdac:`, `rdae:`, `rdaw:`, `rdam:` etcetera that are needed for RDA. 



Work in progress.