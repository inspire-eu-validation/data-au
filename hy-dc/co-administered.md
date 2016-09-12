# Co-administered

**Version**: 1

**Purpose**: Verify whether the adminsteredBy association role is used for administrative units co-administered by two or more administrative units, and the units co-administering this unit apply the inverse role coAdminister.

**Prerequisites**

**Test method**

For each administrative unit co-administered by two or more other administrative units, verify that:
* it refers to these co-administrative units by using the [administeredBy](#administeredBy) association role.
* each of these co-administrative units refers to the mentioned co-administered unit by using the [coAdminister](#coAdminister) association role.

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_AU) IR requirement Section 4.4 (3)

**Test type**: Automatic

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
administeredBy <a name="administeredBy"></a>   | //schema-element(au:AdministrativeUnit)/au:administeredBy
coAdminister  <a name="coAdminister"></a>   | //schema-element(au:AdministrativeUnit)/au:coAdminister


