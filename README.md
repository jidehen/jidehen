### Hi there 👋

My name is Jordan Idehen and I'm a Student a Brown University (Class of 2022), Full-Stack Web Developer, and Software Engineer. I am pursuing an Sc.B degree in Computer Science with specializations in Data and Computational Biology.

Below is my personal profile document written using [RDF-Turtle](https://medium.com/openlink-software-blog/simple-linked-data-deployment-tutorial-a532e568c82f) Notation. 

For maximum effect while viewing my , you are encouraged to install the [OpenLink Structured Data Sniffer Browser Extension](https://chrome.google.com/webstore/detail/openlink-structured-data/egdaiaihbdoiibopledjahjaihbmjhdj?hl=en) (for Chrome and other Web Extensions compliant Browsers) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/openlink-structured-data-sniff/). 

```
## Turtle Start ##

@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix schema: <http://schema.org/> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix cert: <http://www.w3.org/ns/auth/cert#> . 
@prefix : <#> . 

# Profile Document Metadata
<> rdf:type foaf:Document, foaf:PersonalProfileDocument, schema:WebPage, schema:CreativeWork .
<> foaf:maker :i .
<> foaf:primaryTopic :i .
<> schema:mainEntity :i .
<> schema:dateCreated "2020-07-14"^^xsd:dateTime .
<> schema:creator :i .
<> schema:name "Jordan Idehen's Profile Document" .

# Personal Information 
:i schema:mainEntityOfPage <> .
:i schema:mainEntityOfPage <https://www.linkedin.com/in/jordan-idehen-143934157/> .
:i schema:mainEntityOfPage <https://jordanidehen.com/> .
:i rdf:type schema:Person, foaf:Person .
:i schema:name "Jordan Idehen" .
:i owl:sameAs <https://www.linkedin.com/in/jordan-idehen-143934157#this> .

## Turtle End ##
```

Here is an example of a the same document, using [JSON-LD Notaton](https://medium.com/@kidehen/simple-linked-data-deployment-tutorial-using-json-ld-notation-3e753a5d44a3) that's crucial to that effort.

```
## JSON-LD Start ##

{
  "@context": {
    "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
    "foaf": "http://xmlns.com/foaf/0.1/",
    "schema": "http://schema.org/",
    "xsd": "http://www.w3.org/2001/XMLSchema#",
    "owl": "http://www.w3.org/2002/07/owl#"
  },
  "@graph": [
    {
      "@id": "",
      "@type": [
        "foaf:Document",
        "foaf:PersonalProfileDocument",
        "schema:WebPage",
        "schema:CreativeWork"
      ],
      "schema:creator": {
        "@id": "#i"
      },
      "schema:dateCreated": {
        "@type": "xsd:dateTime",
        "@value": "2020-07-14"
      },
      "schema:mainEntity": {
        "@id": "#i"
      },
      "schema:name": "Jordan Idehen's Profile Document",
      "foaf:maker": {
        "@id": "#i"
      },
      "foaf:primaryTopic": {
        "@id": "#i"
      }
    },
    {
      "@id": "#i",
      "@type": [
        "schema:Person",
        "foaf:Person"
      ],
      "schema:mainEntityOfPage": [
        {
          "@id": ""
        },
        {
          "@id": "https://www.linkedin.com/in/jordan-idehen-143934157/"
        },
        {
          "@id": "http://jordanidehen.com"
        },
        
      ],
      "schema:name": "Jordan Idehen",
      "owl:sameAs": [
        {
          "@id": "https://www.linkedin.com/in/jordan-idehen-143934157#this"
        },
      ]
    }
  ]
}

## JSON-LD End ##
```

<!--
**jidehen/jidehen** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

