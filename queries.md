---
layout: page
title: Queries
permalink: /queries/
---
## Retrieve all the protocols with samples that belongs to the *Rodent* order
```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title ?specimenName ?dbpediaDesc
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol ro:has_part ?materials .
  ?materials a sp:MaterialsSection .
  ?materials ro:has_part ?specimens .
  ?specimens a sp:SpecimenList .
  ?specimens ro:has_part ?specimenNameUri .
  ?specimen sp:hasName ?specimenNameUri .
  ?specimenNameUri rdf:value ?specimenName .
  ?specimen owl:sameAs ?externalUri .

  SERVICE <https://dbpedia.org/sparql>
  {
    ?externalUri dbo:order <http://dbpedia.org/resource/Rodent> .
    ?externalUri rdfs:comment ?dbpediaDesc .
    FILTER(lang(?dbpediaDesc) = 'en')
  }
}
```

## Retrieve all the protocols with reagents of type Enzyme
```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title ?name ?desc
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol ro:has_part ?materials .
  ?materials a sp:MaterialsSection .
  ?materials ro:has_part ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagent owl:sameAs ?externalUri .
  ?reagent sp:hasName ?reagentNameUri .
  ?reagentNameUri rdf:value ?name .
  SERVICE <https://dbpedia.org/sparql> {
    ?externalUri a dbo:Enzyme .
    ?externalUri rdfs:comment ?desc .
    FILTER(lang(?desc) = 'en')
  }
}
```

## Retrieve all the protocols with reagents of type Alcohol
```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX yago: <http://dbpedia.org/class/yago/>

SELECT ?title ?name ?desc
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol ro:has_part ?materials .
  ?materials a sp:MaterialsSection .
  ?materials ro:has_part ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagent owl:sameAs ?externalUri .
  ?reagent sp:hasName ?reagentNameUri .
  ?reagentNameUri rdf:value ?name .
  SERVICE <https://dbpedia.org/sparql> {
    ?externalUri a yago:WikicatAlcohols .
    ?externalUri rdfs:comment ?desc.
    FILTER(lang(?desc) = 'en')
  }
}
```

## Retrieve all the reagents along with the different web sites to buy them and all the different manufacturers registered for every reagent
```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX obi: <http://purl.obolibrary.org/obo/OBI_>
PREFIX foaf: <http://xmlns.com/foaf/0.1/>
PREFIX CHEBI: <http://purl.obolibrary.org/obo/CHEBI_>

SELECT ?name
	   (group_concat(?manufacturerName; separator=" , ") as ?manufacturers)
	   (group_concat(?homepage; separator=" , ") as ?whereTobuy)
WHERE {
  ?reagent a CHEBI:33893 .
  ?reagent sp:hasName ?nameUri .
  ?nameUri rdf:value ?name .
  ?reagent obi:0000304 ?manufacturer .
  ?manufacturer sp:hasName ?manufacturerNameUri .
  ?manufacturerNameUri rdf:value ?manufacturerName .
  ?reagent foaf:homepage ?homepage .
} GROUP BY ?name
```

## Retrieve all the protocols with *Fetal bovine serum (FBS)* as a reagent
```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://http://www.obofoundry.org/ro/ro.owl#>

SELECT ?title
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol ro:has_part ?materials .
  ?materials a sp:MaterialsSection .
  ?materials ro:has_part ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagentNameUri rdf:value "Fetal bovine serum (FBS)" .
}
```
