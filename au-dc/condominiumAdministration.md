# Condominium administration

**Version**: 1

**Purpose**: Verify whether each condominium is only administered by administrative units at country level.

**Prerequisites**

**Test method**

Inspect that each [condominium](#condominium) only refers to [administrative units](#AdministrativeUnit) at [country level](#countryLevel) (each of them representing a Member State) through using the [admUnit association role](#admUnit) of the condominium spatial object type.

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (7)

**Test type**: Automatic

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
condominium<a name="condominium"></a>   | //schema-element(au:Condominium)
Administrative Unit <a name="AdministrativeUnit"></a>   | //schema-element(au:AdministrativeUnit)
country level <a name="countryLevel"></a>   | //schema-element(au:AdministrativeUnit)/au:upperLevelUnit
admUnit association role <a name="admUnit"></a>   | //schema-element(au:Condominium)/au:admUnit
