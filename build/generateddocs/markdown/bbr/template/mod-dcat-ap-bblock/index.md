
# MOD-DCAT-Profile (Schema)

`ogc.bbr.template.mod-dcat-ap-bblock` *v0.1*

This Building Block is the DCAT Profile for the MOD ontology

[*Status*](http://www.opengis.net/def/status): Under development

## Description

## MOD-DCAT-Profile

This is the representation of the DCAT Profile for MOD. This document provides a human-readable description of the Profile.

## Examples

### Examples of MOD descriptions complying with the DCAT profile.
This is the content of the example.
#### json
```json
{
    "mod:acronym": "mySA",
    "dct:title": "my semantic artefact",
    "dcat:landingPage": "https://example.org"
}
```

#### json
```json
{
    "mod:hasSyntax": "ttl",
    "mod:hasRepresentationLanguage": "en"
}
```

#### jsonld
```jsonld
{
  "mod:hasSyntax": "ttl",
  "mod:hasRepresentationLanguage": "en",
  "@context": "https://FAIR-IMPACT.github.io/MOD-DCAT-AP-profile/build/annotated/bbr/template/mod-dcat-ap-bblock/context.jsonld"
}
```

#### ttl
```ttl
@prefix mod: <https://w3id.org/mod#> .

[] mod:hasRepresentationLanguage "en" ;
    mod:hasSyntax "ttl" .


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schema for the MOD-DCAT-Profile building block
$defs:
  mod:SemanticArtefact:
    type: object
    properties:
      mod:acronym:
        type: string
      dct:title:
        type: string
      dcat:landingPage:
        type: string
    required:
    - mod:acronym
    - dct:title
    - dcat:landingPage
  mod:SemanticArtefactDistribution:
    type: object
    properties:
      mod:hasSyntax:
        type: string
      mod:hasRepresentationLanguage:
        type: string
anyOf:
- $ref: '#/$defs/mod:SemanticArtefact'
x-jsonld-prefixes:
  mod: https://w3id.org/mod#
  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
  rdfs: http://www.w3.org/2000/01/rdf-schema#
  xsd: http://www.w3.org/2001/XMLSchema#

```

Links to the schema:

* YAML version: [schema.yaml](https://FAIR-IMPACT.github.io/MOD-DCAT-AP-profile/build/annotated/bbr/template/mod-dcat-ap-bblock/schema.json)
* JSON version: [schema.json](https://FAIR-IMPACT.github.io/MOD-DCAT-AP-profile/build/annotated/bbr/template/mod-dcat-ap-bblock/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "mod": "https://w3id.org/mod#",
    "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
    "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
    "xsd": "http://www.w3.org/2001/XMLSchema#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://FAIR-IMPACT.github.io/MOD-DCAT-AP-profile/build/annotated/bbr/template/mod-dcat-ap-bblock/context.jsonld)

## Sources

* [MOD Ontology](https://github.com/fair-IMPACT/mod)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/FAIR-IMPACT/MOD-DCAT-AP-profile](https://github.com/FAIR-IMPACT/MOD-DCAT-AP-profile)
* Path: `_sources/mod-dcat-ap-bblock`

