---
title: MOD-DCAT-Profile (Schema)

language_tabs:
  - json: JSON
  - jsonld: JSON-LD
  - turtle: RDF/Turtle

toc_footers:
  - Version 0.1
  - <a href='#'>MOD-DCAT-Profile</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: MOD-DCAT-Profile (Schema)
---


# MOD-DCAT-Profile `ogc.bbr.template.mod-dcat-bblock`

This Building Block is the DCAT Profile for the MOD ontology

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/FAIR-IMPACT/MOD-DCAT-profile/blob/master/build/tests/bbr/template/mod-dcat-bblock/" target="_blank">valid</a></strong>
</aside>

# Description

## MOD-DCAT-Profile

This is the representation of the DCAT Profile for MOD. This document provides a human-readable description of the Profile.

# Examples

## Examples of MOD descriptions complying with the DCAT profile.

This is the content of the example.



```json
{
    "mod:acronym": "mySA",
    "dct:title": "my semantic artefact"    
}
  
  
  
  
```

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/tests/bbr/template/mod-dcat-bblock/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2FFAIR-IMPACT.github.io%2FMOD-DCAT-profile%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2Fmod-dcat-bblock%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>




```jsonld
{
  "mod:acronym": "mySA",
  "dct:title": "my semantic artefact",
  "@context": "https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/context.jsonld"
}
```

<blockquote class="lang-specific jsonld">
  <p class="example-links">
    <a target="_blank" href="https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/tests/bbr/template/mod-dcat-bblock/example_1_1.jsonld">Open in new window</a>
    <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2FFAIR-IMPACT.github.io%2FMOD-DCAT-profile%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2Fmod-dcat-bblock%2Fexample_1_1.jsonld">View on JSON-LD Playground</a>
</blockquote>




```turtle
@prefix mod: <https://w3id.org/mod#> .
@prefix ns1: <dct:> .

[] ns1:title "my semantic artefact" ;
    mod:acronym "mySA" .


```

<blockquote class="lang-specific turtle">
  <p class="example-links">
    <a target="_blank" href="https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/tests/bbr/template/mod-dcat-bblock/example_1_1.ttl">Open in new window</a>
</blockquote>



# JSON Schema

```yaml--schema
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

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2FFAIR-IMPACT.github.io%2FMOD-DCAT-profile%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2Fmod-dcat-bblock%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/schema.yaml" target="_blank">https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/schema.yaml</a>
* JSON version: <a href="https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/schema.json" target="_blank">https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/schema.json</a>


# JSON-LD Context

```json--ldContext
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

> <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2FFAIR-IMPACT.github.io%2FMOD-DCAT-profile%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2Fmod-dcat-bblock%2Fcontext.jsonld">View on JSON-LD Playground</a>

You can find the full JSON-LD context here:
<a href="https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/context.jsonld" target="_blank">https://FAIR-IMPACT.github.io/MOD-DCAT-profile/build/annotated/bbr/template/mod-dcat-bblock/context.jsonld</a>

# References

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/FAIR-IMPACT/MOD-DCAT-profile" target="_blank">https://github.com/FAIR-IMPACT/MOD-DCAT-profile</a>
* Path:
<code><a href="https://github.com/FAIR-IMPACT/MOD-DCAT-profile/blob/HEAD/_sources/mod-dcat-bblock" target="_blank">_sources/mod-dcat-bblock</a></code>

