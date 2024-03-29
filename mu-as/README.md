# Conformance class: Application schema, Administrative Units - Maritime Units

Conformance class for the requirements associated with the application schema. 

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Administrative Units - Maritime Units".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Administrative Units](http://inspire.ec.europa.eu/id/ats/data-au).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AU](#ref_TG_DS_AU) | [GML application schemas, Administrative Units](../au-gml) | INSPIRE spatial data set encoded in GML, Administrative Units features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types in the application schema are:

* Baseline
* MaritimeBoundary
* MaritimeZone

*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AU <a name="ref_TG_DS_AU"></a>   | [INSPIRE Data Specification on Administrative Units – Technical Guidelines version](https://knowledge-base.inspire.ec.europa.eu/publications/inspire-data-specification-administrative-units-technical-guidelines_en)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](https://knowledge-base.inspire.ec.europa.eu/publications/data-specifications-template_en)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AU](#ref_TG_DS_AU)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code list values](./code-list-values.md)  | Draft  | A.1.3  |
| [Constraints](./constraints.md)  | Draft  | A.1.6  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
net          | http://inspire.ec.europa.eu/schemas/net/4.0
mu           | http://inspire.ec.europa.eu/schemas/mu/4.0
au          | http://inspire.ec.europa.eu/schemas/au/5.0
net            | http://inspire.ec.europa.eu/schemas/net/4.0
base           | http://inspire.ec.europa.eu/schemas/base/4.0
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace

