<div rel="foaf:primaryTopic" resource="#" typeof="owl:Ontology">

Author  
<a href="https://doriantaylor.com/person/dorian-taylor#me"
rel="dct:creator" typeof="foaf:Person"><span property="foaf:name">Dorian
Taylor</span></a>

Created  
September 6, 2023

Namespace URI  
[`https://vocab.methodandstructure.com/cache-metadata#`](https://vocab.methodandstructure.com/cache-metadata#)

Preferred Namespace Prefix  
`cm`

This vocabulary is intended to describe the metadata necessary to
positively identify HTTP cache entries.

</div>

<div id="ch.classes" class="section" rel="dct:hasPart"
resource="#ch.classes" typeof="bibo:DocumentPart">

## Classes

<div id="Entry" class="section" about="cm:Entry" typeof="owl:Class">

### `Entry`

The class `cm:Entry` represents (canonically) an individual HTTP cache
entry.

Subclass of:  
<a href="https://www.w3.org/TR/prov-o/#Entity" rel="rdfs:subClassOf"
resource="prov:Entity"><code>prov:Entity</code></a>

Properties:  
<a href="https://vocab.methodandstructure.com/cache-metadata#resource"
rev="rdfs:domain"><code>cm:resource</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#principal"
rev="rdfs:domain"><code>cm:principal</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#header"
rev="rdfs:domain"><code>cm:header</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

</div>

<div id="ch.properties" class="section" rel="dct:hasPart"
resource="#ch.properties" typeof="bibo:DocumentPart">

## Properties

<div id="resource" class="section" about="cm:resource"
typeof="owl:ObjectProperty">

### `resolver`

This property maps the `itcv:Engine` to an `itcv:Resolver`.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:domain"><code>cm:Entry</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

</div>

<div id="ch.references" class="section" rel="dct:hasPart"
resource="#ch.references" typeof="bibo:DocumentPart">

## References

- <a href="https://www.w3.org/TR/HTTP-in-RDF10/" rel="rdfs:seeAlso"><span
  property="dct:title">HTTP Vocabulary in RDF 1.0</span></a>
- <a href="https://www.w3.org/TR/prov-o/" rel="rdfs:seeAlso"><span
  property="dct:title">PROV-O: The PROV Ontology</span></a>
- <a href="https://pav-ontology.github.io/pav/" rel="rdfs:seeAlso"><span
  property="dct:title">PAV — Provenance, Authoring and
  Versioning</span></a>

</div>
