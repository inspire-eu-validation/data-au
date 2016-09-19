# Boundary

**Version**: 1

**Purpose**: Verify whether all instances of the spatial object type administrative boundary correspond to the edges in the topological structure of the complete (including all levels) boundary graph.

**Prerequisites**

**Test method**

For each administrative unit not corresponding to the lowest [level of the administrative hierarchy](#nationalLevel), verify that:
* it refers to all its respective lower level administrative units in the administrative hierarchy.
* this reference is expressed using the [lowerLevelUnit](#lowerLevelUnit) association role of the administrative unit spatial object type.

Inspect that the [geometry](#geometry) of each instance [administrative boundary](#AdministrativeBoundary) correspond to an edge in the topological structure formed by the complete boundary graph, including the boundaries of all levels.

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (5)

**Test type**: Automatic

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
AdministrativeBoundary <a name="AdministrativeBoundary"></a>   | //schema-element(au:AdministrativeBoundary
geometry <a name="geometry"></a>  | $AdministrativeBoundary/*:geometry
