
# MOD-DCAT-Profile (Schema)

`ogc.bbr.template.mod-dcat-bblock` *v0.1*

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
    "dct:title": "my semantic artefact"    
}
  
  
  
  
```

#### jsonld
```jsonld
{
  "mod:acronym": "mySA",
  "dct:title": "my semantic artefact",
  "@context": "https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/context.jsonld"
}
```

#### ttl
```ttl
@prefix mod: <https://w3id.org/mod#> .
@prefix ns1: <dct:> .

[] ns1:title "my semantic artefact" ;
    mod:acronym "mySA" .


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schema for the MOD-DCAT-Profile building block
$defs:
  SemanticArtefact:
    type: object
    properties:
      mod:acronym:
        type: string
      dct:title:
        type: string
    required:
    - mod:acronym
    - dct:title
anyOf:
- $ref: '#/$defs/SemanticArtefact'
x-jsonld-prefixes:
  mod: https://w3id.org/mod#
  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
  rdfs: http://www.w3.org/2000/01/rdf-schema#
  xsd: http://www.w3.org/2001/XMLSchema#

```

Links to the schema:

* YAML version: [schema.yaml](https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/schema.json)
* JSON version: [schema.json](https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/schema.yaml)


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
[context.jsonld](https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/context.jsonld)

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/FAIR-IMPACT/MOD-DCAT-profile](https://github.com/FAIR-IMPACT/MOD-DCAT-profile)
* Path: `_sources/mod-dcat-bblock`

