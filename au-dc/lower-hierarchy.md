# Lower Hierarchy

**Version**: 1

**Purpose**: Verify that administrative units, except those corresponding to the lowest level, refer to its respective lower level units in the administrative hierarchy.

**Prerequisites**

**Test method**

For each administrative unit not corresponding to the lowest [level of the administrative hierarchy](#nationalLevel), verify that:
* it refers to a lower level administrative unit using the [lowerLevelUnit](#lowerLevelUnit) association role.
* it refers to lower level administrative units on the next level using the [lowerLevelUnit](#lowerLevelUnit) association role.

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (1)
* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (2)

**Test type**: Automatic

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
lowerLevelUnit <a name="lowerLevelUnit"></a>   | //schema-element(au:AdministrativeUnit)/au:lowerLevelUnit
level of the administrative hierarchy  <a name="nationalLevel"></a>   | //schema-element(au:AdministrativeUnit)/au:nationalLevel

