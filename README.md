# RIBS - RDA Improved By Simplification

Goal of RIBS is to make it easier to work with RDA (Resource Description and Access) metadata standard in an RDF based context.

This is done by

* Getting rid of all elements (properties) that refer to any of the subclasses of <http://rdaregistry.info/Elements/c/C10002> ("Agent") and have a super-property that can replace them.
* Getting rid of all cryptical properties and classes like `rdac:C10008` and `rdae:P20319` and replacing them by something more human friendly like `ribs:Family` and `ribs:aggregates.`
* Aggregating all definitions into one, allowing to use just one namespace prefix '`ribs:`' in stead of the many like `rdac:`, `rdae:`, `rdaw:`, `rdam:` etcetera that are needed for RDA. 



Work in progress.