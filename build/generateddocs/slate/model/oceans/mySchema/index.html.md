---
title: My Schema (Schema)

language_tabs:
  - json: JSON
  - jsonld: JSON-LD
  - turtle: RDF/Turtle
  - shell
  - python: Python
  - javascript: Javascript

toc_footers:
  - Version 0.1
  - <a href='#'>My Schema</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: My Schema (Schema)
---


# My Schema `ogc.model.oceans.mySchema`

An example schema defining the set of properties of any type of object.

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/ocean-info-model/blob/master/build/tests/model/oceans/mySchema/" target="_blank">valid</a></strong>
</aside>

# Description

## My Schema

Defines a set of properties that may be used in **any** JSON schema.

> Note these properties may be used in the "properties" sub-component of a GeoJSON object, as a simple object

The numeric properties "b" and "c" have an example SHACL rule that if c is present, then c > b
# Examples

## This is an example with just a description and no code snippets.



```json
{
  "@context": {
    "mynamespace": "http://example.org/ns1/"
  },
  "a": "mynamespace:aThing",
  "b": 23,
  "c": 1
}


```

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/ocean-info-model/build/tests/model/oceans/mySchema/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Focean-info-model%2Fbuild%2Ftests%2Fmodel%2Foceans%2FmySchema%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>




```jsonld
{
  "@context": [
    "https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/context.jsonld",
    {
      "mynamespace": "http://example.org/ns1/"
    }
  ],
  "a": "mynamespace:aThing",
  "b": 23,
  "c": 1
}
```

<blockquote class="lang-specific jsonld">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/ocean-info-model/build/tests/model/oceans/mySchema/example_1_1.jsonld">Open in new window</a>
    <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Focean-info-model%2Fbuild%2Ftests%2Fmodel%2Foceans%2FmySchema%2Fexample_1_1.jsonld">View on JSON-LD Playground</a>
</blockquote>




```turtle
@prefix mynamespace: <http://example.org/ns1/> .
@prefix ns1: <https://example.org/my-bb-model/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] a mynamespace:aThing ;
    ns1:b 23 ;
    ns1:c 1 .


```

<blockquote class="lang-specific turtle">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/ocean-info-model/build/tests/model/oceans/mySchema/example_1_1.ttl">Open in new window</a>
</blockquote>


This an example.

In **Markdown** format.


## Examples can have content and/or code snippets.



```shell
echo 'Hello, world!'
```



```python
print('Hello, world!')
```



```javascript
console.log('Hello, world!')
```

The content of this example. 


# JSON Schema

```yaml--schema
$schema: https://json-schema.org/draft/2020-12/schema
description: My example schema
type: object
properties:
  a:
    type: string
    format: uri
    x-jsonld-id: '@type'
  b:
    type: number
    x-jsonld-id: https://example.org/my-bb-model/b
  c:
    type: number
    x-jsonld-id: https://example.org/my-bb-model/c
required:
- a
- b

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Focean-info-model%2Fbuild%2Fannotated%2Fmodel%2Foceans%2FmySchema%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/schema.yaml" target="_blank">https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/schema.json" target="_blank">https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/schema.json</a>


# JSON-LD Context

```json--ldContext
{
  "@context": {
    "a": "@type",
    "b": "https://example.org/my-bb-model/b",
    "c": "https://example.org/my-bb-model/c",
    "@version": 1.1
  }
}
```

> <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Focean-info-model%2Fbuild%2Fannotated%2Fmodel%2Foceans%2FmySchema%2Fcontext.jsonld">View on JSON-LD Playground</a>

You can find the full JSON-LD context here:
<a href="https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/context.jsonld" target="_blank">https://ogcincubator.github.io/ocean-info-model/build/annotated/model/oceans/mySchema/context.jsonld</a>

# Validation

## SHACL Shapes

The following sets of SHACL shapes are used for validating this building block:

* My Schema <small><code>ogc.model.oceans.mySchema</code></small>
  * [https://ogcincubator.github.io/ocean-info-model/_sources/mySchema/rules.shacl](https://ogcincubator.github.io/ocean-info-model/_sources/mySchema/rules.shacl)

# References

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/ocean-info-model" target="_blank">https://github.com/ogcincubator/ocean-info-model</a>
* Path:
<code><a href="https://github.com/ogcincubator/ocean-info-model/blob/HEAD/_sources/mySchema" target="_blank">_sources/mySchema</a></code>

