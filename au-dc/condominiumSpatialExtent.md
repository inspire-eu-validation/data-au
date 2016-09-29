# Condominium spatial extent

**Version**: 1

**Purpose**: Verify whether the spatial extent of a condominium is not part of the geometry representing the spatial extent of an administrative unit.

**Prerequisites**

**Test method**

Inspect each [condominium](#condominium)  and verify that its [geometry](#geometryCondominium) does not overlap with the [geometry](#geometryAdministrativeUnit) of any of the [administrative units](#AdministrativeUnit) in the same data set.

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (6)

**Test type**: Automatic

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
condominium<a name="condominium"></a>   | //schema-element(au:condominium)
geometry Condominium <a name="geometryCondominium"></a>   | $condominium/*:geometry
Administrative Unit <a name="AdministrativeUnit"></a>   | //schema-element(au:AdministrativeUnit)
geometry Administrative Unit <a name="geometryAdministrativeUnit"></a>  | $AdministrativeUnit/*:geometry
