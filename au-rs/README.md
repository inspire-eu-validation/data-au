# Conformance class: Reference systems, Administrative Units (DRAFT)

Conformance class for the requirements associated with reference systems (spatial and temporal, units of measurement).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schema for Administrative Units".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Administrative Units](http://inspire.ec.europa.eu/id/ats/data-au/3.2).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [Reference systems](https://github.com/inspire-eu-validation/data/tree/master/reference-systems) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AU](#ref_TG_DS_AU) | [GML application schema, Administrative Units Simple](../au-gml) | INSPIRE spatial data set encoded in GML, Administrative Units features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types are:
 
* ProtectedSite
 
*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AU <a name="ref_TG_DS_au"></a>   | [INSPIRE Data Specification on Administrative Units – Technical Guidelines version 3.2](https://knowledge-base.inspire.ec.europa.eu/publications/inspire-data-specification-administrative-units-technical-guidelines_en)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](https://knowledge-base.inspire.ec.europa.eu/publications/data-specifications-template_en)

## Test Cases

None, all reference system test cases are covered by the generic [Reference systems](https://github.com/inspire-eu-validation/data/tree/master/reference-systems) tests.

## XML namespace prefixes <a name="namespaces"></a>

n/a
