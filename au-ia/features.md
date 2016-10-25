# Feature references

**Version**: 1

**Purpose**: Verify that referenced features can be retrieved.

**Prerequisites**

**Test method**

* Verify that any feature reference in an association role is publicly accessible via HTTP, i.e. inspect all relevant properties. If a reference (@xlink:href) has a value that starts with "#", verify that an element with a `gml:id` attribute with the referenced identifier exists in the same document. If the reference starts with "http", verify that a HTTP GET request to the URI retrieves an XML document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following association roles:

* AdministrativeUnit.[NUTS](#NUTS) : NUTSRegion
* AdministrativeUnit.[condominium](#condominium) : Condominium
* AdministrativeUnit.[upperLevelUnit](#upperLevelUnit) : AdministrativeUnit
* AdministrativeUnit.[administeredBy](#administeredBy) : AdministrativeUnit
* AdministrativeUnit.[coAdminister](#coAdminister) : AdministrativeUnit
* AdministrativeUnit.[boundary](#boundary) : AdministrativeBoundary
* AdministrativeBoundary.[admUnit](#admUnit) : AdministrativeUnit
* Condominium.[admUnit](#admUnit) : AdministrativeUnit


**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-ia/README#ref_TG_DS_tmpl) IR requirement Article 4 (2)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-ia/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
NUTS <a name ="NUTS"></a>	| //schema-element(au:AdministrativeUnit)/stat:NUTSregion/@xlink:href
condominium <a name ="condominium"></a>	| //schema-element(au:AdministrativeUnit)/au:Condominium/@xlink:href
upperLevelUnit <a name ="upperLevelUnit"></a>	| //schema-element(au:AdministrativeUnit)/au:upperLevelUnit/@xlink:href
administeredBy <a name ="administeredBy"></a>	| //schema-element(au:AdministrativeUnit)/au:administeredBy/@xlink:href
coAdminister <a name ="coAdminister"></a>	| //schema-element(au:AdministrativeUnit)/au:coAdminister/@xlink:href
boundary <a name ="boundary"></a>	| //schema-element(au:AdministrativeBoundary)/au:boundary/@xlink:href
admUnit <a name ="admUnit"></a>	| //schema-element(au:AdministrativeBoundary)/au:admUnit/@xlink:href and //schema-element(au:Condominium)/au:admUnit/@xlink:href
