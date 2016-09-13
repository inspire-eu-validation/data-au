# Higher Hierarchy

**Version**: 1

**Purpose**: Verify that administrative units, except those corresponding to the country level unit representing a Member State or being a co-administered unit, refer to exactly one administrative unit at a higher level of administrative hierarchy.

**Prerequisites**

**Test method**

For each administrative unit, except those corresponding to the [Country Level unit](#CountryLevel) representing a Member State or being a [co-administered unit](#coAdminister), verify that:
* it refers to exactly one administrative unit at a higher level of administrative hierarchy, i.e. there is only one administrative unit spatial object at the [UpperLevelUnit](#UpperLevelUnit) association role of the administrative Unit.

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
UpperLevelUnit <a name="UpperLevelUnit"></a>   | //schema-element(au:AdministrativeUnit)/au:upperLevelUnit
Country level unit <a name="CountryLevel"></a>   | //schema-element(au:AdministrativeUnit)/au:nationalLevel
coAdministered unit <a name="coAdminister"></a>   | //schema-element(au:AdministrativeUnit)/au:coAdminister

