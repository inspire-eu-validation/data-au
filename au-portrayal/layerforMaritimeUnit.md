# Layer for Maritime Unit

**Purpose**: For each Maritime Unit zone type, one layer of those specified in section 11 shall be provided

**Prerequisites**

**Test method**

* check whether one [layer name](#name) following the [template AU.<CodelistValue>](#names) is provided for each [Maritime Unit zone](#zone) type used in the data set.

**Reference(s)**:

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-portrayal/README#ref_TG_DS_AU), IR Requirement, Article 14(1)(a)

**Test type**: Automated

**Notes**

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-portrayal/README#namespaces).

Abbreviation                                     |  XPath expression												|  Parameter  value
------------------------------------------------ | ---------------------------------------------------------------	| ---------------------------------------------------------------
Maritime Unit Zone <a name="zone"></a> | //schema-element(mu:MaritimeZone)
layer name <a name="name"></a> | /wms:WMS_Capabilities/wms:Capability/wms:Layer/wms:Name | ISO 19128
                                 | /wmts:Capabilities/wmts:Contents/wmts:Layer/ows:Identifier | WMTS 1.0.0
template AU.<CodelistValue> <a name="names"></a> | ('AU.ContiguousZone', 'AU.ContinentalShelf', 'AU.ExclusiveEconomicZone', 'AU.InternalWaters', 'AU.TerritorialSea')
