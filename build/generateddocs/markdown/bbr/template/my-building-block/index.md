
# MOD-DCAT-Profile (Schema)

`ogc.bbr.template.my-building-block` *v0.1*

This Building Block is the DCAT Profile for the MOD ontology

[*Status*](http://www.opengis.net/def/status): Under development

## Description

## MOD-DCAT-Profile

This is the representation of the DCAT Profile for MOD. This document provides a human-readable description of the Profile.

## Examples

### This is an example with just a description and no code snippets.
This is the content of the example.

In **Markdown** format.

### Examples can have content and/or code snippets.
The content of this example. 
#### shell
```shell
echo 'Hello, world!'
```

#### python
```python
print('Hello, world!')
```

#### javascript
```javascript
console.log('Hello, world!')
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schema for the MOD-DCAT-Profile building block
type: object
properties:
  a:
    type: string
    format: uri
  b:
    type: number
required:
- a
- b
x-jsonld-prefixes:
  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
  rdfs: http://www.w3.org/2000/01/rdf-schema#
  xsd: http://www.w3.org/2001/XMLSchema#

```

Links to the schema:

* YAML version: [schema.yaml](https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/my-building-block/schema.json)
* JSON version: [schema.json](https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/my-building-block/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
    "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
    "xsd": "http://www.w3.org/2001/XMLSchema#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/my-building-block/context.jsonld)

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/FAIR-IMPACT/MOD-DCAT-profile](https://github.com/FAIR-IMPACT/MOD-DCAT-profile)
* Path: `_sources/my-building-block`

