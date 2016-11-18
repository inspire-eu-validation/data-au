# Code list values

**Version**: 1

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

When an attribute has a code list as its type, verify that the values comply with the definitions and include the values set out in Annex II of the regulation. To pass this tests that any instance of an attribute

* takes only values explicitly specified in the INSPIRE code list register when the code list‘s extensibility is 'none'.

Otherwise report [disallowedCodeListValue](#disallowedCodeListValue).

In the Administrative Units - Maritime Units application schema, the following properties have to be tested:
* [MaritimeZoneType (v3)](#zoneType3). Valid values:
  * contiguousZone
  * internalWaters
  * territorialSea
  * exclusiveEconomicZone
  * continentalShelf
* [MaritimeZoneType (v4)](#zoneType4). Valid values:
  * http://inspire.ec.europa.eu/codelist/MaritimeZoneTypeValue/contiguousZone
  * http://inspire.ec.europa.eu/codelist/MaritimeZoneTypeValue/continentalShelf
  * http://inspire.ec.europa.eu/codelist/MaritimeZoneTypeValue/exclusiveEconomicZone
  * http://inspire.ec.europa.eu/codelist/MaritimeZoneTypeValue/internalWaters
  * http://inspire.ec.europa.eu/codelist/MaritimeZoneTypeValue/territorialSea
* [BaselineSegmentType (v3)](#segmentType3). Valid values:
  * normal
  * straight
  * archipelagic
* [BaselineSegmentType (v4)](#segmentType4). Valid values:
  * http://inspire.ec.europa.eu/codelist/BaselineSegmentTypeValue/archipelagic
  * http://inspire.ec.europa.eu/codelist/BaselineSegmentTypeValue/normal
  * http://inspire.ec.europa.eu/codelist/BaselineSegmentTypeValue/straight


The following is not applicable for this application schema as no extensions are allowed. It is still included here as a reminder in case extensions will be allowed in the future:

Inspect the code list valued property elements. If a value is not one of the values listed above, review the code list definition to check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements. This is a manual test.
  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
BaselineSegmentType (v3) <a name="#segmentType3"></a>   | //schema-element(mu:BaselineProperty/mu:segmentType/text()
BaselineSegmentType (v4) <a name="#segmentType4"></a>   | //schema-element(mu:BaselineProperty/mu:segmentType/@href:xlink
MaritimeZoneType (v3) <a name="#zoneType3"></a>   | //schema-element(mu:MaritimeZone/mu:zoneType/text()
MaritimeZoneType (v4) <a name="#zoneType4"></a>   | //schema-element(mu:MaritimeZone/mu:zoneType/@href:xlink
