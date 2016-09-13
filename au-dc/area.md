# Area

**Version**: 1

**Purpose**: Verify whether administrative units having the same level of administrative hierarchy do not conceptually share common areas.

**Prerequisites**

**Test method**

* Verify that the [geometry of each administrative unit](#geometry) does not overlap with the geometries of other administrative units having the same [level of administrative hierarchy](#nationalLevel) as the examined one.

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (4)

**Test type**: Automatic

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
geometry of administrative unit <a name="geometry"></a>   | //schema-element(au:AdministrativeUnit)/au:geometry
level of administrative hierarchy <a name="nationalLevel"></a>   | //schema-element(au:AdministrativeUnit)/au:nationalLevel

