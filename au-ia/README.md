# Conformance class: Information accessibility, Administrative Units

Conformance class for the requirements related to the accessibility of referenced information, for example, information stored in registries (code lists, coordinate reference systems).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Administrative Units".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Administrative Units](http://inspire.ec.europa.eu/id/ats/data-au/3.1).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [Information accessibility](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AU](#ref_TG_DS_HY) | [GML application schemas, Administrative Units](../au-gml) | INSPIRE spatial data set encoded in GML, Administrative Units features | n/a |
 
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
TG DS-AU <a name="ref_TG_DS_AU"></a>   | [INSPIRE Data Specification on Administrative Units – Technical Guidelines](https://knowledge-base.inspire.ec.europa.eu/publications/inspire-data-specification-administrative-units-technical-guidelines_en)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](https://knowledge-base.inspire.ec.europa.eu/publications/data-specifications-template_en)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AU](#ref_TG_DS_AU)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code lists](./code-list.md)  | ready for review  | A.6.1 |
| [Feature references](./features.md)  | ready for review  | A.1.4 |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gml            | http://www.opengis.net/gml/3.2
au          | http://inspire.ec.europa.eu/schemas/au/5.0
mu      			| http://inspire.ec.europa.eu/schemas/mu/4.0

The following variables are used to refer to the corresponding Xpath expressions in all test descriptions:

Variable       | Value
-------------- | -------------------------------------------------
$features      |  //schema-element(au:AdministrativeBoundary) \| //schema-element(au:AdministrativeUnit) \| //schema-element(au:Condominium) \| //schema-element(mu:Baseline) \| //schema-element(mu:MaritimeBoundary) \| //schema-element(mu:MaritimeZone)
