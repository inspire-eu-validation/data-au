# Basic test

**Version**: 1

**Purpose**: Verify that the spatial data set contains at least one Administrative Units feature.

**Prerequisites**

**Test method**

* Check that the set of [features](#features) in the spatial data set is not empty. Otherwise report [noFeature](#noFeature)

**Reference(s)**: 

* [TG DS-AU](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-gml/README#ref_TG_DS_AU) 5.4, 5.5

**Test type**: Automated

**Notes**

There is no requirement that we could reference in the Technical Guidelines, but such a requirement is clearly missing for any data set with hydrographic features. Maybe such a requirement should be added in the future revision?

## Messages

Identifier  |  Message text (parameters start with '$')
----------- | -------------------------------------------------------------------------
noFeature <a name="noFeature"/>  |  	The XML documents representing the spatial data set do not contain a feature of any of the spatial object types in the 'Administrative Units - Administrative Units' or 'Administrative Units - Maritime Units' application schemas. Therefore, the spatial data set cannot conform to this conformance class. If you have expected to find spatial objects from the application schema in the data set, please consult the statistics information to see the spatial object types that have been found.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-gml/README#namespaces).

Abbreviation                                          |  XPath expression
----------------------------------------------------- | ------------------------------------------------------------------
features <a name="features"></a>   |  //schema-element(au:AdministrativeBoundary) \| //schema-element(au:AdministrativeUnit) \| //schema-element(au:Condominium) \| //schema-element(mu:Baseline) \| //schema-element(mu:MaritimeBoundary) \| //schema-element(mu:MaritimeZone)