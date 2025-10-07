<div rel="foaf:primaryTopic" resource="#" typeof="owl:Ontology">

Author  
<a href="https://doriantaylor.com/person/dorian-taylor#me"
rel="dct:creator" typeof="foaf:Person"><span property="foaf:name">Dorian
Taylor</span></a>

Created  
October 3, 2025

Namespace URI  
[`https://vocab.methodandstructure.com/cache-metadata#`](https://vocab.methodandstructure.com/cache-metadata#)

Preferred Namespace Prefix  
`cache`

This vocabulary is intended to describe the metadata necessary to
positively identify HTTP cache entries.

    @prefix cache: <https://vocab.methodandstructure.com/cache-metadata#> .
    @prefix tfo:   <https://vocab.methodandstructure.com/transformation#> .
    @prefix ht:    <http://www.w3.org/2011/http#> .
    @prefix hth:   <http://www.w3.org/2011/http-headers#> .
    @prefix htm:   <http://www.w3.org/2011/http-methods#> .
    @prefix prov:  <http://www.w3.org/ns/prov#> .
    @prefix xsd:   <http://www.w3.org/2001/XMLSchema#> .

    <urn:uuid:b30c0e75-6b53-4212-8b95-a04629aa03d9> a cache:Entry ;
      cache:entity <ni:///sha-256;ocz5wuIt2_E5vOW_DqPkJSONCUg61TPJ8c81fBKH5co> ;
      cache:expires "2025-10-07T01:52:07Z"^^xsd:dateTime ;
      cache:header [
        a ht:RequestHeader ;
        ht:hdrName hth:accept ;
        ht:fieldName "Accept";
        ht:fieldValue "text/html, application/xhtml+xml, */*;q=0.1" ], [
        a ht:RequestHeader ;
        ht:hdrName hth:accept-language ;
        ht:fieldName "Accept-Language";
        ht:fieldValue "en-us, en, fr;q=0.8" ] ;
      cache:method htm:GET ;
      cache:origin <https://internet.home/page> ;
      cache:principal <mailto:some@personal.email> ;
      cache:private true ;
      dct:format "text/html"^^tfo:content-type ;
      dct:language "en"^^xsd:token ;
      dct:modified "2025-10-07T01:22:07Z"^^xsd:dateTime ;
      prov:generatedAtTime "2025-10-07T01:22:07Z"^^xsd:dateTime .

</div>

<div id="ch.classes" class="section" rel="dct:hasPart"
resource="#ch.classes" typeof="bibo:DocumentPart">

## Classes

<figure>
<img
src="https://vocab.methodandstructure.com/cache-metadata-classes" />
</figure>

<div id="Entry" class="section" about="cache:Entry" typeof="owl:Class">

### `Entry`

The class `cache:Entry` represents (canonically) an individual HTTP
cache entry.

Subclass of:  
<a href="https://www.w3.org/TR/prov-o/#Entity" rel="rdfs:subClassOf"
resource="prov:Entity"><code>prov:Entity</code></a>

Properties:  
<a href="https://vocab.methodandstructure.com/cache-metadata#resource"
rev="rdfs:domain"><code>cache:resource</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#principal"
rev="rdfs:domain"><code>cache:principal</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#header"
rev="rdfs:domain"><code>cache:header</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

</div>

<div id="ch.properties" class="section" rel="dct:hasPart"
resource="#ch.properties" typeof="bibo:DocumentPart">

## Properties

<figure>
<img
src="https://vocab.methodandstructure.com/cache-metadata-properties" />
</figure>

<div id="entity" class="section" about="cache:entity"
typeof="owl:ObjectProperty">

### `entity`

This denotes the actual literal representation of the cache entry.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#Entry"
rel="rdfs:domain"><code>cache:Entry</code></a>

Range:  
<a href="https://www.w3.org/TR/rdf-schema/#ch_resource" rel="rdfs:range"
resource="rdfs:Resource"><code>rdfs:Resource</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

<div id="expires" class="section" about="cache:expires"
typeof="owl:DatatypeProperty">

### `expires`

The `xsd:dateTime` when the cache expires.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#Entry"
rel="rdfs:domain"><code>cache:Entry</code></a>

Range:  
<a href="https://www.w3.org/TR/xmlschema11-2/#dateTime" rel="rdfs:range"
resource="xsd:dateTime"><code>xsd:dateTime</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

<div id="header" class="section" about="cache:header"
typeof="owl:ObjectProperty">

### `header`

Denotes an individual HTTP header.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#Entry"
rel="rdfs:domain"><code>cache:Entry</code></a>

Range:  
<a href="https://www.w3.org/TR/HTTP-in-RDF10/#MessageHeaderClass"
rel="rdfs:range"
resource="ht:MessageHeader"><code>ht:MessageHeader</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

<div id="method" class="section" about="cache:method"
typeof="owl:ObjectProperty">

### `method`

Denotes the HTTP method of the associated request.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#Entry"
rel="rdfs:domain"><code>cache:Entry</code></a>

Range:  
<a href="https://www.w3.org/TR/HTTP-in-RDF10/#MethodClass"
rel="rdfs:range" resource="ht:Method"><code>ht:Method</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

<div id="origin" class="section" about="cache:origin"
typeof="owl:ObjectProperty">

### `origin`

This relates the cache entry to the origin resource that was retrieved.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#Entry"
rel="rdfs:domain"><code>cache:Entry</code></a>

Range:  
<a href="https://www.w3.org/TR/rdf-schema/#ch_resource" rel="rdfs:range"
resource="rdfs:Resource"><code>rdfs:Resource</code></a>

<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:isDefinedBy">Back to Top</a>

</div>

<div id="principal" class="section" about="cache:principal"
typeof="owl:ObjectProperty">

### `principal`

This relates the cache entry to the origin resource that was retrieved.

Domain:  
<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:domain"><code>cache:Entry</code></a>

Range:  
<a href="https://vocab.methodandstructure.com/cache-metadata#"
rel="rdfs:range"><code>rdfs:Resource</code></a>

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
