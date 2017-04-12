---
layout: page
title: Queries
permalink: /queries/
---
1. [Retrieve all the protocols with samples that belongs to the *Rodent* order](#1-retrieve-all-the-protocols-with-samples-that-belongs-to-the-rodent-order)
2. [Retrieve all the protocols with reagents of type Enzyme](#2-retrieve-all-the-protocols-with-reagents-of-type-enzyme)
3. [Retrieve all the protocols with reagents of type Alcohol](#3-retrieve-all-the-protocols-with-reagents-of-type-alcohol)
4. [Retrieve all the reagents along with the different web sites to buy them and all the different manufacturers registered for every reagent](#4-retrieve-all-the-reagents-along-with-the-different-web-sites-to-buy-them-and-all-the-different-manufacturers-registered-for-every-reagent)
5. [Retrieve all the protocols with Fetal bovine serum (FBS) as a reagent](#5-retrieve-all-the-protocols-with-fetal-bovine-serum-fbs-as-a-reagent)
6. [Retrieve the application of the protocol titled “Extraction of total RNA from fresh/frozen tissue (FT)”](#6-retrieve-the-application-of-the-protocol-titled-extraction-of-total-rna-from-freshfrozen-tissue-ft)
7. [Retrieve the procedure labels involved in the protocol titled “Extraction of total RNA from fresh/frozen tissue (FT)”](#7-retrieve-the-procedure-labels-involved-in-the-protocol-titled-extraction-of-total-rna-from-freshfrozen-tissue-ft)
8. [Retrieve the purpose of the protocol titled “Isolation of Lung Infiltrating Cell in Mice”](#8-retrieve-the-purpose-of-the-protocol-titled-isolation-of-lung-infiltrating-cell-in-mice)
9. [Retrieve the reagent list and equipment and supplies list of the protocol titled “Isolation of Lung Infiltrating Cell in Mice”](#9-retrieve-the-reagent-list-and-equipment-and-supplies-list-of-the-protocol-titled-isolation-of-lung-infiltrating-cell-in-mice)
10. [Retrieve the protocols that use the reagents “Dulbecco’s modified eagle medium (DMEM)”, “Fetal bovine serum (FBS)” and “Phosphate buffered saline (PBS)”](#10-retrieve-the-protocols-that-use-the-reagents-dulbeccos-modified-eagle-medium-dmem-fetal-bovine-serum-fbs-and-phosphate-buffered-saline-pbs)
11. [Retrieve all the protocols that contains Mouse as a Sample](#11-retrieve-all-the-protocols-that-contains-mouse-as-a-sample)
12. [Retrieve all the instruments and reagents used in the protocol “Mouse Retinal Whole Mounts and Quantification of Vasculature Protocol”](#12-retrieve-all-the-instruments-and-reagents-used-in-the-protocol-mouse-retinal-whole-mounts-and-quantification-of-vasculature-protocol)
13. [Retrieve all the protocols that use the software “ImageJ” along wiht its homepage (http://rsb.info.nih.gov/ij/download.html).](#13-retrieve-all-the-protocols-that-use-the-software-imagej-along-wiht-its-homepage-httprsbinfonihgovijdownloadhtml)



## 1. Retrieve all the protocols with samples that belongs to the *Rodent* order
### Makes use of external resources, federated query
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0APREFIX+dbo%3A+%3Chttp%3A%2F%2Fdbpedia.org%2Fontology%2F%3E%0D%0A%0D%0ASELECT+%3Ftitle+%3FspecimenName%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Fspecimens+.%0D%0A++%3Fspecimens+a+sp%3ASpecimenList+.%0D%0A++%3Fspecimens+ro%3Ahas_part+%3FspecimenNameUri.%0D%0A++%3FspecimenNameUri+rdf%3Avalue+%3FspecimenName+.%0D%0A++%3Fspecimen+sp%3AhasName+%3FspecimenNameUri.%0D%0A++SERVICE+%3Chttps%3A%2F%2Fdbpedia.org%2Fsparql%3E%0D%0A++%7B%0D%0A++++%3FexternalUri+dbo%3Aorder+%3Chttp%3A%2F%2Fdbpedia.org%2Fresource%2FRodent%3E+.%0D%0A++++%3FexternalUri+rdfs%3Acomment+%3FdbpediaDesc+.%0D%0A++++FILTER%28lang%28%3FdbpediaDesc%29+%3D+%27en%27%29%0D%0A++%7D%0D%0A++%3Fspecimen+owl%3AsameAs+%3FexternalUri+.%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title ?specimenName
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?specimens .
  ?specimens a sp:SpecimenList .
  ?specimens ro:has_part ?specimenNameUri.
  ?specimenNameUri rdf:value ?specimenName .
  ?specimen sp:hasName ?specimenNameUri.
  SERVICE <https://dbpedia.org/sparql>
  {
    ?externalUri dbo:order <http://dbpedia.org/resource/Rodent> .
    ?externalUri rdfs:comment ?dbpediaDesc .
    FILTER(lang(?dbpediaDesc) = 'en')
  }
  ?specimen owl:sameAs ?externalUri .
}
```

## 2. Retrieve all the protocols with reagents of type Enzyme
### Makes use of external resources, federated query
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0APREFIX+dbo%3A+%3Chttp%3A%2F%2Fdbpedia.org%2Fontology%2F%3E%0D%0A%0D%0ASELECT+%3Ftitle+%3Fname+%3Fdesc%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23has_part%3E+%3FreagentNameUri.%0D%0A++%3Freagent+owl%3AsameAs+%3FexternalUri+.%0D%0A++%3Freagent+sp%3AhasName+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3Fname+.%0D%0A++SERVICE+%3Chttps%3A%2F%2Fdbpedia.org%2Fsparql%3E+%7B%0D%0A++++%3FexternalUri+a+dbo%3AEnzyme+.%0D%0A++++%3FexternalUri+rdfs%3Acomment+%3Fdesc+.%0D%0A++++FILTER%28lang%28%3Fdesc%29+%3D+%27en%27%29%0D%0A++%7D%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>


```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title ?name ?desc
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri.
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

## 3. Retrieve all the protocols with reagents of type Alcohol
### Makes use of external resources, federated query
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0APREFIX+yago%3A+%3Chttp%3A%2F%2Fdbpedia.org%2Fclass%2Fyago%2F%3E%0D%0A%0D%0ASELECT+%3Ftitle+%3Fname+%3Fdesc%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3Freagent+owl%3AsameAs+%3FexternalUri+.%0D%0A++%3Freagent+sp%3AhasName+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3Fname+.%0D%0A++SERVICE+%3Chttps%3A%2F%2Fdbpedia.org%2Fsparql%3E+%7B%0D%0A++++%3FexternalUri+a+yago%3AWikicatAlcohols+.%0D%0A++++%3FexternalUri+rdfs%3Acomment+%3Fdesc+.%0D%0A++++FILTER%28lang%28%3Fdesc%29+%3D+%27en%27%29%0D%0A++%7D%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX yago: <http://dbpedia.org/class/yago/>

SELECT ?title ?name ?desc
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagent owl:sameAs ?externalUri .
  ?reagent sp:hasName ?reagentNameUri .
  ?reagentNameUri rdf:value ?name .
  SERVICE <https://dbpedia.org/sparql> {
    ?externalUri a yago:WikicatAlcohols .
    ?externalUri rdfs:comment ?desc .
    FILTER(lang(?desc) = 'en')
  }
}
```

## 4. Retrieve all the reagents along with the different web sites to buy them and all the different manufacturers registered for every reagent.
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0APREFIX+obi%3A+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FOBI_%3E%0D%0APREFIX+foaf%3A+%3Chttp%3A%2F%2Fxmlns.com%2Ffoaf%2F0.1%2F%3E%0D%0APREFIX+CHEBI%3A+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FCHEBI_%3E%0D%0A%0D%0ASELECT+%3Fname%0D%0A%09+++%28group_concat%28%3FmanufacturerName%3B+separator%3D%22+%2C+%22%29+as+%3Fmanufacturers%29%0D%0A%09+++%28group_concat%28%3Fhomepage%3B+separator%3D%22+%2C+%22%29+as+%3FreagentHomepage%29%0D%0AWHERE+%7B%0D%0A++%3Freagent+a+CHEBI%3A33893+.%0D%0A++%3Freagent+sp%3AhasName+%3FnameUri+.%0D%0A++%3FnameUri+rdf%3Avalue+%3Fname+.%0D%0A++%3Freagent+obi%3A0000304+%3Fmanufacturer+.%0D%0A++%3Fmanufacturer+sp%3AhasName+%3FmanufacturerNameUri+.%0D%0A++%3FmanufacturerNameUri+rdf%3Avalue+%3FmanufacturerName+.%0D%0A++%3Freagent+foaf%3Ahomepage+%3Fhomepage+.%0D%0A%7D+GROUP+BY+%3Fname&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

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
     (group_concat(?homepage; separator=" , ") as ?reagentHomepage)
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

## 5. Retrieve all the protocols with *Fetal bovine serum (FBS)* as a reagent
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0A%0D%0ASELECT+%3Ftitle%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%22Fetal+bovine+serum+%28FBS%29%22+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>

SELECT ?title
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagentNameUri rdf:value "Fetal bovine serum (FBS)" .
}
```

## 6. Retrieve the application of the protocol titled “Extraction of total RNA from fresh/frozen tissue (FT)”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0A%0D%0ASELECT+%3FprotocolApplication%0D%0A%7B%0D%0A++++%3Fprotocol+sp%3AhasTitle+%3FtitleUri+.%0D%0A++++%3FtitleUri+rdf%3Avalue+%22Extraction+of+total+RNA+from+fresh%2Ffrozen+tissue+%28FT%29%22+.%0D%0A++++%3Fprotocol+sp%3AhasApplication+%3FapplicationUri+.%0D%0A++++%3FapplicationUri+rdf%3Avalue+%3FprotocolApplication+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?protocolApplication
{
    ?protocol sp:hasTitle ?titleUri .
    ?titleUri rdf:value "Extraction of total RNA from fresh/frozen tissue (FT)" .
    ?protocol sp:hasApplication ?applicationUri .
    ?applicationUri rdf:value ?protocolApplication .
} 
```

## 7. Retrieve the procedure labels involved in the protocol titled “Extraction of total RNA from fresh/frozen tissue (FT)”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0A%0D%0ASELECT+%3FprocedureLabel%0D%0A%7B%0D%0A++++%3FexperimentalProtocol+sp%3AhasTitle+%3FtitleUri+.%0D%0A++++%3FtitleUri+rdf%3Avalue+%22Extraction+of+total+RNA+from+fresh%2Ffrozen+tissue+%28FT%29%22+.%0D%0A++++%3FexperimentalProtocolExecution+sp%3AdocumentedIn+%3FexperimentalProtocol+.%0D%0A++++%3FexperimentalProtocolExecution+sp%3AhasProcedure+%3Fprocedure+.%0D%0A++++%3Fprocedure+rdfs%3Alabel+%3FprocedureLabel+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?procedureLabel
{
    ?experimentalProtocol sp:hasTitle ?titleUri .
    ?titleUri rdf:value "Extraction of total RNA from fresh/frozen tissue (FT)" .
    ?experimentalProtocolExecution sp:documentedIn ?experimentalProtocol .
    ?experimentalProtocolExecution sp:hasProcedure ?procedure .
    ?procedure rdfs:label ?procedureLabel .
}
```

## 8. Retrieve the purpose of the protocol titled “Isolation of Lung Infiltrating Cell in Mice”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0A%0D%0ASELECT+%3FprotocolPurpose%0D%0A%7B%0D%0A++++%3Fprotocol+sp%3AhasTitle+%3FtitleUri+.%0D%0A++++%3FtitleUri+rdf%3Avalue+%22Isolation+of+Lung+Infiltrating+Cell+in+Mice%22+.%0D%0A++++%3Fprotocol+sp%3AhasPurpose+%3FpurposeUri+.%0D%0A++++%3FpurposeUri+rdf%3Avalue+%3FprotocolPurpose+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?protocolPurpose
{
    ?protocol sp:hasTitle ?titleUri .
    ?titleUri rdf:value "Isolation of Lung Infiltrating Cell in Mice" .
    ?protocol sp:hasPurpose ?purposeUri .
    ?purposeUri rdf:value ?protocolPurpose .
}
```

## 9. Retrieve the reagent list and equipment and supplies list of the protocol titled “Isolation of Lung Infiltrating Cell in Mice”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0A%0D%0ASELECT+%28group_concat%28distinct%28%3FreagentName%29%3Bseparator%3D%22+%7C+%22%29+as+%3FprotocolReagents%29%0D%0A+++++++%28group_concat%28distinct%28%3FequipmentName%29%3Bseparator%3D%22+%7C+%22%29+as+%3FprotocolInstruments%29%0D%0AWHERE+%7B%0D%0A++++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++++%3Ftitle_uri+rdf%3Avalue+%22Isolation+of+Lung+Infiltrating+Cell+in+Mice%22+.%0D%0A++++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++++%3Freagents+a+sp%3AReagentList+.%0D%0A++++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++++%3Fprotocol+sp%3AhasExperimentalInput+%3Fequipment+.%0D%0A++++%3Fequipment+a+sp%3AEquipmentAndSuppliesList+.%0D%0A++++%3Fequipment+ro%3Ahas_part+%3FequipmentNameUri+.%0D%0A++++%3FequipmentNameUri+rdf%3Avalue+%3FequipmentName+.%0D%0A%7D+GROUP+BY+%3Fprotocol&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

``` 
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>

SELECT (group_concat(distinct(?reagentName);separator=" | ") as ?protocolReagents)
       (group_concat(distinct(?equipmentName);separator=" | ") as ?protocolInstruments)
WHERE {
    ?protocol sp:hasTitle ?title_uri .
    ?title_uri rdf:value "Isolation of Lung Infiltrating Cell in Mice" .
    ?protocol sp:hasExperimentalInput ?reagents .
    ?reagents a sp:ReagentList .
    ?reagents ro:has_part ?reagentNameUri .
    ?reagentNameUri rdf:value ?reagentName .
    ?protocol sp:hasExperimentalInput ?equipment .
    ?equipment a sp:EquipmentAndSuppliesList .
    ?equipment ro:has_part ?equipmentNameUri .
    ?equipmentNameUri rdf:value ?equipmentName .
} GROUP BY ?protocol
```

## 10. Retrieve the protocols that use the reagents “Dulbecco's modified eagle medium (DMEM)”, “Fetal bovine serum (FBS)” and “Phosphate buffered saline (PBS)”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+prism%3A+%3Chttp%3A%2F%2Fprismstandard.org%2Fnamespaces%2Fbasic%2F2.0%2Fprism%3A%3E%0D%0A%0D%0ASELECT+DISTINCT+%3Fidentifier+%3Ftitle+%3FpublicationName%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasIdentifier+%3FprotocolIdentifier+.%0D%0A++%3FprotocolIdentifier+rdf%3Avalue+%3Fidentifier+.%0D%0A++%3Fprotocol+sp%3ApublishedIn+%3Fpublication+.%0D%0A++%3Fpublication+sp%3AhasName+%3FpublicationNameUri+.%0D%0A++%3FpublicationNameUri+rdf%3Avalue+%3FpublicationName+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri1+.%0D%0A++%3FreagentNameUri1+rdf%3Avalue+%22Fetal+bovine+serum+%28FBS%29%22+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri2+.%0D%0A++%3FreagentNameUri2+rdf%3Avalue+%22Dulbecco%27s+modified+eagle+medium+%28DMEM%29%22+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri3+.%0D%0A++%3FreagentNameUri3+rdf%3Avalue+%22Phosphate+buffered+saline+%28PBS%29%22+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX prism: <http://prismstandard.org/namespaces/basic/2.0/prism:>

SELECT DISTINCT ?identifier ?title ?publicationName
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasIdentifier ?protocolIdentifier .
  ?protocolIdentifier rdf:value ?identifier .
  ?protocol sp:publishedIn ?publication .
  ?publication sp:hasName ?publicationNameUri .
  ?publicationNameUri rdf:value ?publicationName .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri1 .
  ?reagentNameUri1 rdf:value "Fetal bovine serum (FBS)" .
  ?reagents ro:has_part ?reagentNameUri2 .
  ?reagentNameUri2 rdf:value "Dulbecco's modified eagle medium (DMEM)" .
  ?reagents ro:has_part ?reagentNameUri3 .
  ?reagentNameUri3 rdf:value "Phosphate buffered saline (PBS)" .
}
```

## 11. Retrieve all the protocols that contains Mouse as a Sample
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+p-plan%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2Fp-plan%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+foaf%3A+%3Chttp%3A%2F%2Fxmlns.com%2Ffoaf%2F0.1%2F%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0APREFIX+dbo%3A+%3Chttp%3A%2F%2Fdbpedia.org%2Fontology%2F%3E%0D%0A%0D%0ASELECT+%3Ftitle+%3Fname%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Fspecimens+.%0D%0A++%3Fspecimens+a+sp%3ASpecimenList+.%0D%0A++%3Fspecimens+ro%3Ahas_part+%3FspecimenNameUri+.%0D%0A++%3FspecimenNameUri+rdf%3Avalue+%3Fname+.%0D%0A++%3Fspecimen+sp%3AhasName+%3FspecimenNameUri+.%0D%0A++%3Fspecimen+owl%3AsameAs+%3Chttp%3A%2F%2Fdbpedia.org%2Fresource%2FMouse%3E+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX p-plan: <http://purl.org/net/p-plan#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX foaf: <http://xmlns.com/foaf/0.1/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title ?name
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?specimens .
  ?specimens a sp:SpecimenList .
  ?specimens ro:has_part ?specimenNameUri .
  ?specimenNameUri rdf:value ?name .
  ?specimen sp:hasName ?specimenNameUri .
  ?specimen owl:sameAs <http://dbpedia.org/resource/Mouse> .
}
```

## 12. Retrieve all the instruments and reagents used in the protocol “Mouse Retinal Whole Mounts and Quantification of Vasculature Protocol”

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX p-plan: <http://purl.org/net/p-plan#>
PREFIX ro: <http://http://www.obofoundry.org/ro/ro.owl#>
PREFIX foaf: <http://xmlns.com/foaf/0.1/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?reagentName
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Mouse Retinal Whole Mounts and Quantification of Vasculature Protocol" .
  ?protocol ro:hasPart ?materials .
  ?materials a sp:MaterialsSection .
  ?materials ro:hasPart ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:hasPart ?reagent .
  ?reagent sp:hasName ?nameUri .
  ?nameUri rdf:value ?reagentName .
}
```

## 13. Retrieve all the protocols that use the software "ImageJ" along wiht its homepage (http://rsb.info.nih.gov/ij/download.html).

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX p-plan: <http://purl.org/net/p-plan#>
PREFIX ro: <http://http://www.obofoundry.org/ro/ro.owl#>
PREFIX foaf: <http://xmlns.com/foaf/0.1/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title  ?download
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol ro:hasPart ?materials .
  ?materials a sp:MaterialsSection .
  ?materials ro:hasPart ?softwareList .
  ?softwareList a sp:SoftwareList .
  ?softwareList ro:hasPart ?software .
  ?software sp:hasName ?nameUri .
  ?nameUri rdf:value "ImageJ software" .
  ?software foaf:homepage ?download .
}
```



