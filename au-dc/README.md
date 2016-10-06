# Conformance class: Data consistency, Administrative Units (DRAFT)

Conformance class for the requirements related to the consistency of the data.

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has a direct dependency to the conformance class "INSPIRE GML application schemas".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Administrative Units](http://inspire.ec.europa.eu/id/ats/data-au/3.1).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-dc/README#ref_TG_DS_tmpl) | [Data consistency](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/data-consistency) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

 
## Feature types <a name="feature-types"></a>

The instantiable feature types are:

AdministrativeUnits:

* AdministrativeBoundary
* AdministrativeUnit
* Condominium

MaritimeUnits:

* Baseline
* MaritimeBoundary
* MaritimeZone

*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AU <a name="ref_TG_DS_AU"></a>   | [INSPIRE Data Specification on Administrative Units – Technical Guidelines version 3.1](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_AU_v3.1.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AU](#ref_TG_DS_AU)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Area consistency](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/area)  | ready for review  | A.3.8  |
| [Boundary consistency](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/boundary)  | ready for review  | A.3.9  |
| [Co-administered consistency](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/co-administered)  | ready for review  | A.3.7  |
| [Condominium administration](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/condominiumAdministration)  | ready for review  | A.3.11  |
| [Condominium spatial extent](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/condominiumSpatialExtent)  | ready for review  | A.3.10  |
| [Higher hierarchy consistency](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/higher-hierarchy)  | ready for review  | A.3.5  |
| [Lower hierarchy consistency](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/hy-dc/lower-hierarchy)  | ready for review  | A.3.6  |


## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
au          | http://inspire.ec.europa.eu/schemas/au/4.0 or urn:x-inspire:specification:gmlas:AdministrativeUnits:3.0
au3          | urn:x-inspire:specification:gmlas:AdministrativeUnits:3.0
gml            | http://www.opengis.net/gml/3.2
