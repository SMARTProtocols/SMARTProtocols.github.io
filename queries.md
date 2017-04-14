---
layout: page
title: Competency questions
permalink: /queries/
---
1. [Retrieve all the protocols with samples that belongs to the *Rodent* order](#1-retrieve-all-the-protocols-with-samples-that-belongs-to-the-rodent-order)  
Makes use of external resources, federated query
2. [Retrieve all the protocols with reagents of type Enzyme](#2-retrieve-all-the-protocols-with-reagents-of-type-enzyme)  
Makes use of external resources, federated query
3. [Retrieve all the protocols with reagents of type Alcohol](#3-retrieve-all-the-protocols-with-reagents-of-type-alcohol)  
Makes use of external resources, federated query
4. [Retrieve all the reagents along with the different web sites to buy them and all the different manufacturers registered for every reagent](#4-retrieve-all-the-reagents-along-with-the-different-web-sites-to-buy-them-and-all-the-different-manufacturers-registered-for-every-reagent)
5. [Retrieve all the protocols with Fetal bovine serum (FBS) as a reagent](#5-retrieve-all-the-protocols-with-fetal-bovine-serum-fbs-as-a-reagent)
6. [Retrieve the application of the protocol titled “Extraction of total RNA from fresh/frozen tissue (FT)”](#6-retrieve-the-application-of-the-protocol-titled-extraction-of-total-rna-from-freshfrozen-tissue-ft)
7. [Retrieve the procedure labels involved in the protocol titled “Extraction of total RNA from fresh/frozen tissue (FT)”](#7-retrieve-the-procedure-labels-involved-in-the-protocol-titled-extraction-of-total-rna-from-freshfrozen-tissue-ft)
8. [Retrieve the purpose of the protocol titled “Isolation of Lung Infiltrating Cell in Mice”](#8-retrieve-the-purpose-of-the-protocol-titled-isolation-of-lung-infiltrating-cell-in-mice)
9. [Retrieve all the instruments and reagents used in the protocol “Mouse Retinal Whole Mounts and Quantification of Vasculature Protocol”](#9-retrieve-all-the-instruments-and-reagents-used-in-the-protocol-mouse-retinal-whole-mounts-and-quantification-of-vasculature-protocol)
10. [Retrieve the protocols that use the reagents “Dulbecco’s modified eagle medium (DMEM)”, “Fetal bovine serum (FBS)” and “Phosphate buffered saline (PBS)”](#10-retrieve-the-protocols-that-use-the-reagents-dulbeccos-modified-eagle-medium-dmem-fetal-bovine-serum-fbs-and-phosphate-buffered-saline-pbs)
11. [Retrieve all the protocols that contains Mouse as a Sample](#11-retrieve-all-the-protocols-that-contains-mouse-as-a-sample)
12. [Retrieve all the protocols that use the software “ImageJ” along wiht its homepage (http://rsb.info.nih.gov/ij/download.html).](#12-retrieve-all-the-protocols-that-use-the-software-imagej-along-wiht-its-homepage-httprsbinfonihgovijdownloadhtml)
13. [Retrieve all the reagents manufactured by Sigma-Aldrich in protocol "Isolation of Lung Infiltrating Cell in Mice"](#13-retrieve-all-the-reagents-manufactured-by-sigma-aldrich-in-protocol-isolation-of-lung-infiltrating-cell-in-mice)
14. [Retrieve all the diseases caused by the reagents in the protocol “Extraction of total RNA from fresh/frozen tissue (FT)”](#14-retrieve-all-the-diseases-caused-by-the-reagents-in-the-protocol-extraction-of-total-rna-from-freshfrozen-tissue-ft)  
Makes use of external resources, federated query  
15. [Retrieve all the protocols with “Schizosaccharomyces pombe” in their samples lists](#15-retrieve-all-the-protocols-with-schizosaccharomyces-pombe-in-their-samples-lists)  
16. [Retrieve the protocols that include 2 or more procedures](#16-retrieve-the-protocols-that-include-2-or-more-procedures)  
17. [Retrieve the critical steps included in the protocol titled “[Bio101] Subcutaneous Injection of Tumor Cells”](#17-retrieve-the-critical-steps-included-in-the-protocol-titled-bio101-subcutaneous-injection-of-tumor-cells)
18. [Retrieve the advantages and limitations of the protocol titled “Defining transcribed regions using RNA-seq”](#18-retrieve-the-advantages-and-limitations-of-the-protocol-titled-defining-transcribed-regions-using-rna-seq)  
19. [Retrieve the recipe list of the protocol titled “Defining transcribed regions using RNA-seq”](#19-retrieve-the-recipe-list-of-the-protocol-titled-defining-transcribed-regions-using-rna-seq) 
20. [For the protocol titled “Defining transcribed regions using RNA-seq”, give me the steps that include cautions as alert message and the materials participating in such step](#20-for-the-protocol-titled-defining-transcribed-regions-using-rna-seq-give-me-the-steps-that-include-cautions-as-alert-message-and-the-materials-participating-in-such-step)  
21. [Retrieve the provenance of the protocol titled “Scratch Wound Healing Assay”
](#21-retrieve-the-provenance-of-the-protocol-titled-scratch-wound-healing-assay) 
22. [Retrieve the specimen names that could be tested in the protocols titled “A simplified universal genomic DNA extraction protocol suitable for PCR” and “RNA Isolation from Synechocystis”](#22-retrieve-the-specimen-names-that-could-be-tested-in-the-protocols-titled-a-simplified-universal-genomic-dna-extraction-protocol-suitable-for-pcr-and-rna-isolation-from-synechocystis)  
23. [Retrieve the protocols and the list of reagents for documents authored by Yanling Chen](#23-retrieve-the-protocols-and-the-list-of-reagents-for-documents-authored-by-yanling-chen)  
24. [Retrieve the protocols authored by Cristian Olaya and Wilmer Cuellar using Cassava (NCBITAXON:3983) as a sample](#24-retrieve-the-protocols-authored-by-cristian-olaya-and-wilmer-cuellar-using-cassava-ncbitaxon3983-as-a-sample)
25. [Retrieve the common reagents across the protocols “[Bio101] Subcutaneous Injection of Tumor Cells” and “Scratch Wound Healing Assay”](#25-retrieve-the-common-reagents-across-the-protocols-bio101-subcutaneous-injection-of-tumor-cells-and-scratch-wound-healing-assay)
26. [Retrieve the protocols in which Bromophenol blue is used and tell me about the application of Bromophenol blue](#26-retrieve-the-protocols-in-which-bromophenol-blue-is-used-and-tell-me-about-the-application-of-bromophenol-blue)







## 1. Retrieve all the protocols with samples that belongs to the *Rodent* order  
Makes use of external resources, federated query  

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
Makes use of external resources, federated query  

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
Makes use of external resources, federated query  

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
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0A%0D%0ASELECT+%3FprocedureLabel%0D%0A%7B%0D%0A++++%3FexperimentalProtocol+sp%3AhasTitle+%3FtitleUri+.%0D%0A++++%3FtitleUri+rdf%3Avalue+%22Extraction+of+total+RNA+from+fresh%2Ffrozen+tissue+%28FT%29%22+.%0D%0A++++%3FexperimentalProtocolExecution+sp%3AisDocumentedIn+%3FexperimentalProtocol+.%0D%0A++++%3FexperimentalProtocolExecution+sp%3AhasProcedure+%3Fprocedure+.%0D%0A++++%3Fprocedure+rdfs%3Alabel+%3FprocedureLabel+.%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?procedureLabel
{
    ?experimentalProtocol sp:hasTitle ?titleUri .
    ?titleUri rdf:value "Extraction of total RNA from fresh/frozen tissue (FT)" .
    ?experimentalProtocolExecution sp:isDocumentedIn ?experimentalProtocol .
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

## 9. Retrieve all the instruments and reagents used in the protocol “Mouse Retinal Whole Mounts and Quantification of Vasculature Protocol”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0A%0D%0ASELECT+%28group_concat%28distinct%28%3FreagentName%29%3Bseparator%3D%22+%7C+%22%29+as+%3FprotocolReagents%29%0D%0A+++++++%28group_concat%28distinct%28%3FequipmentName%29%3Bseparator%3D%22+%7C+%22%29+as+%3FprotocolInstruments%29%0D%0AWHERE+%7B%0D%0A++++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++++%3Ftitle_uri+rdf%3Avalue+%22Mouse+Retinal+Whole+Mounts+and+Quantification+of+Vasculature+Protocol%22+.%0D%0A++++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++++%3Freagents+a+sp%3AReagentList+.%0D%0A++++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++++%3Fprotocol+sp%3AhasExperimentalInput+%3Fequipment+.%0D%0A++++%3Fequipment+a+sp%3AEquipmentAndSuppliesList+.%0D%0A++++%3Fequipment+ro%3Ahas_part+%3FequipmentNameUri+.%0D%0A++++%3FequipmentNameUri+rdf%3Avalue+%3FequipmentName+.%0D%0A%7D+GROUP+BY+%3Fprotocol&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

``` 
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>

SELECT (group_concat(distinct(?reagentName);separator=" | ") as ?protocolReagents)
       (group_concat(distinct(?equipmentName);separator=" | ") as ?protocolInstruments)
WHERE {
    ?protocol sp:hasTitle ?title_uri .
    ?title_uri rdf:value "Mouse Retinal Whole Mounts and Quantification of Vasculature Protocol" .
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

## 12. Retrieve all the protocols that use the software "ImageJ" along wiht its homepage (http://rsb.info.nih.gov/ij/download.html).
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+p-plan%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2Fp-plan%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+foaf%3A+%3Chttp%3A%2F%2Fxmlns.com%2Ffoaf%2F0.1%2F%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0APREFIX+dbo%3A+%3Chttp%3A%2F%2Fdbpedia.org%2Fontology%2F%3E%0D%0A%0D%0ASELECT+%3Ftitle++%3Fdownload%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3FsoftwareList+.%0D%0A++%3FsoftwareList+a+sp%3ASoftwareList+.%0D%0A++%3FsoftwareList+ro%3Ahas_part+%3FsoftwareNameUri+.%0D%0A++%3Fsoftware+sp%3AhasName+%3FsoftwareNameUri+.%0D%0A++%3FsoftwareNameUri+rdf%3Avalue+%22ImageJ+software%22+.%0D%0A++%3Fsoftware+foaf%3Ahomepage+%3Fdownload+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX p-plan: <http://purl.org/net/p-plan#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX foaf: <http://xmlns.com/foaf/0.1/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT ?title  ?download
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?softwareList .
  ?softwareList a sp:SoftwareList .
  ?softwareList ro:has_part ?softwareNameUri .
  ?software sp:hasName ?softwareNameUri .
  ?softwareNameUri rdf:value "ImageJ software" .
  ?software foaf:homepage ?download .
}
```

## 13. Retrieve all the reagents manufactured by Sigma-Aldrich in protocol "Isolation of Lung Infiltrating Cell in Mice"
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+obi%3A+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FOBI_%3E%0D%0A%0D%0ASELECT+%3FreagentName%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22Isolation+of+Lung+Infiltrating+Cell+in+Mice%22+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3Freagent+sp%3AhasName+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++%3Freagent+obi%3A0000304+%3Fmanufacturer+.%0D%0A++%3Fmanufacturer+sp%3AhasName+%3FmanufacturerNameUri+.%0D%0A++%3FmanufacturerNameUri+rdf%3Avalue+%22Sigma-Aldrich%22+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX obi: <http://purl.obolibrary.org/obo/OBI_>

SELECT ?reagentName
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Isolation of Lung Infiltrating Cell in Mice" .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagent sp:hasName ?reagentNameUri .
  ?reagentNameUri rdf:value ?reagentName .
  ?reagent obi:0000304 ?manufacturer .
  ?manufacturer sp:hasName ?manufacturerNameUri .
  ?manufacturerNameUri rdf:value "Sigma-Aldrich" .
}
```

## 14. Retrieve all the diseases caused by the reagents in the protocol "Extraction of total RNA from fresh/frozen tissue (FT)”  
Makes use of external resources, federated query  
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0A%0D%0ASELECT+%3FreagentName+%3FreagentSame+%3FdiseaseLabel%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22Extraction+of+total+RNA+from+fresh%2Ffrozen+tissue+%28FT%29%22+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++%3Freagent+sp%3AhasName+%3FreagentNameUri+.%0D%0A++%3Freagent+owl%3AsameAs+%3FreagentSame+.%0D%0A++%0D%0A++SERVICE+%3Chttp%3A%2F%2Fsparql.bioontology.org%2Fontologies%2Fsparql%2F%3Fapikey%3INSERT YOUR API KEY HERE%3E+%7B%0D%0A++++%3FreagentSame+%3Chttp%3A%2F%2Fpurl.bioontology.org%2Fontology%2FSNOMEDCT%2Fcausative_agent_of%3E+%3FdiseaseUri.%0D%0A++++%3FdiseaseUri+%3Chttp%3A%2F%2Fwww.w3.org%2F2004%2F02%2Fskos%2Fcore%23prefLabel%3E+%3FdiseaseLabel+.%0D%0A++%7D%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  


```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>

SELECT ?reagentName ?reagentSame ?diseaseLabel
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Extraction of total RNA from fresh/frozen tissue (FT)" .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagentNameUri rdf:value ?reagentName .
  ?reagent sp:hasName ?reagentNameUri .
  ?reagent owl:sameAs ?reagentSame .
  
  SERVICE <http://sparql.bioontology.org/ontologies/sparql/?apikey=INSERT YOUR API KEY HERE> {
    ?reagentSame <http://purl.bioontology.org/ontology/SNOMEDCT/causative_agent_of> ?diseaseUri.
    ?diseaseUri <http://www.w3.org/2004/02/skos/core#prefLabel> ?diseaseLabel .
  }
}
```

## 15. Retrieve all the protocols with “Schizosaccharomyces pombe” in their samples lists
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E+%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0A%0D%0ASELECT+%3Ftitle%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Fspecimens+.%0D%0A++%3Fspecimens+a+sp%3ASpecimenList+.%0D%0A++%3Fspecimens+ro%3Ahas_part+%3FspecimenNameUri+.%0D%0A++%3FspecimenNameUri+rdf%3Avalue+%22Schizosaccharomyces+pombe%22+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#> 
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?title
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?specimens .
  ?specimens a sp:SpecimenList .
  ?specimens ro:has_part ?specimenNameUri .
  ?specimenNameUri rdf:value "Schizosaccharomyces pombe" .
}
```

## 16. Retrieve the protocols that include 2 or more procedures
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0A%0D%0ASELECT+%3Ftitle%0D%0A%7B%0D%0A++++%3FexperimentalProtocol+sp%3AhasTitle+%3FtitleUri+.%0D%0A++++%3FtitleUri+rdf%3Avalue+%3Ftitle+.%0D%0A++++%3FexperimentalProtocolExecution+sp%3AisDocumentedIn+%3FexperimentalProtocol+.%0D%0A++++%3FexperimentalProtocolExecution+sp%3AhasProcedure+%3Fprocedure+.%0D%0A++++%0D%0A%7D+GROUP+BY+%3Ftitle+HAVING+%28COUNT%28%3Fprocedure%29+%3E+1%29&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?title
{
    ?experimentalProtocol sp:hasTitle ?titleUri .
    ?titleUri rdf:value ?title .
    ?experimentalProtocolExecution sp:isDocumentedIn ?experimentalProtocol .
    ?experimentalProtocolExecution sp:hasProcedure ?procedure .
    
} GROUP BY ?title HAVING (COUNT(?procedure) > 1)
```

## 17. Retrieve the critical steps included in the protocol titled “[Bio101] Subcutaneous Injection of Tumor Cells”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0A%0D%0ASELECT+%3FsubprocedureDesc+%3FcriticalStepDescription%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22%5BBio101%5D+Subcutaneous+Injection+of+Tumor+Cells%22+.%0D%0A++%3FprotocolExecution+sp%3AisDocumentedIn+%3Fprotocol+.%0D%0A++%3FprotocolExecution+sp%3AhasProcedure+%3Fprocedure+.%0D%0A++%3Fprocedure+sp%3AhasSubprocedure+%3Fsubprocedure+.%0D%0A++%3Fsubprocedure+sp%3AhasAlertMessage+%3FcriticalStep+.%0D%0A++%3Fsubprocedure+sp%3AhasDescription+%3FsubprocedureDescUri+.%0D%0A++%3FsubprocedureDescUri+rdf%3Avalue+%3FsubprocedureDesc+.%0D%0A++%3FcriticalStep+a+sp%3ACriticalStep+.%0D%0A++%3FcriticalStep+rdf%3Avalue+%3FcriticalStepDescription+.%0D%0A%7D&should-sponge=grab-all&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?subprocedureDesc ?criticalStepDescription
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "[Bio101] Subcutaneous Injection of Tumor Cells" .
  ?protocolExecution sp:isDocumentedIn ?protocol .
  ?protocolExecution sp:hasProcedure ?procedure .
  ?procedure sp:hasSubprocedure ?subprocedure .
  ?subprocedure sp:hasAlertMessage ?criticalStep .
  ?subprocedure sp:hasDescription ?subprocedureDescUri .
  ?subprocedureDescUri rdf:value ?subprocedureDesc .
  ?criticalStep a sp:CriticalStep .
  ?criticalStep rdf:value ?criticalStepDescription .
}
```

## 18. Retrieve the advantages and limitations of the protocol titled “Defining transcribed regions using RNA-seq”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0A%0D%0ASELECT+%3Fadvantage+%3Flimitation%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22Defining+transcribed+regions+using+RNA-seq%22+.%0D%0A++%3Fprotocol+sp%3AhasAdvantage+%3FadvantageUri+.%0D%0A++%3Fprotocol+sp%3AhasLimitation+%3FlimitationUri+.%0D%0A++%3FadvantageUri+rdf%3Avalue+%3Fadvantage+.%0D%0A++%3FlimitationUri+rdf%3Avalue+%3Flimitation+.%0D%0A++%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?advantage ?limitation
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Defining transcribed regions using RNA-seq" .
  ?protocol sp:hasAdvantage ?advantageUri .
  ?protocol sp:hasLimitation ?limitationUri .
  ?advantageUri rdf:value ?advantage .
  ?limitationUri rdf:value ?limitation .
  
}
```

## 19. Retrieve the recipe list of the protocol titled “Defining transcribed regions using RNA-seq”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0A%0D%0ASELECT+%3FrecipeName%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22Defining+transcribed+regions+using+RNA-seq%22+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Frecipes+.%0D%0A++%3Frecipes+a+sp%3ARecipeList+.%0D%0A++%3Frecipes+ro%3Ahas_part+%3FrecipeNameUri+.%0D%0A++%3FrecipeNameUri+rdf%3Avalue+%3FrecipeName+.%0D%0A++%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>

SELECT ?recipeName
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Defining transcribed regions using RNA-seq" .
  ?protocol sp:hasExperimentalInput ?recipes .
  ?recipes a sp:RecipeList .
  ?recipes ro:has_part ?recipeNameUri .
  ?recipeNameUri rdf:value ?recipeName .
}
```

## 20. For the protocol titled “Defining transcribed regions using RNA-seq”, give me the steps that include cautions as alert message and the materials participating in such step
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0D%0A%0D%0ASELECT+%3FsubprocedureDesc+%3FcautionDescription%0D%0A+++++++%28group_concat%28%3FreagentName%3B+separator%3D%22+%2C+%22%29+as+%3FreagentsNames%29%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22Defining+transcribed+regions+using+RNA-seq%22+.%0D%0A++%3FprotocolExecution+sp%3AisDocumentedIn+%3Fprotocol+.%0D%0A++%3FprotocolExecution+sp%3AhasProcedure+%3Fprocedure+.%0D%0A++%3Fprocedure+sp%3AhasSubprocedure+%3Fsubprocedure+.%0D%0A++%3Fsubprocedure+sp%3AhasAlertMessage+%3Fcaution+.%0D%0A++%3Fsubprocedure+sp%3AhasDescription+%3FsubprocedureDescUri+.%0D%0A++%3FsubprocedureDescUri+rdf%3Avalue+%3FsubprocedureDesc+.%0D%0A++%3Fcaution+a+%3Chttp%3A%2F%2Fwww.owl-ontologies.com%2FOntology1184060740.owl%23Class_122%3E+.%0D%0A++%3Fcaution+rdf%3Avalue+%3FcautionDescription+.%0D%0A++%3FreagentNameUri+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FRO_0000056%3E+%3Fsubprocedure+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A%7D+GROUP+BY+%3FsubprocedureDesc+%3FcautionDescription&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?subprocedureDesc ?cautionDescription
       (group_concat(?reagentName; separator=" , ") as ?reagentsNames)
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Defining transcribed regions using RNA-seq" .
  ?protocolExecution sp:isDocumentedIn ?protocol .
  ?protocolExecution sp:hasProcedure ?procedure .
  ?procedure sp:hasSubprocedure ?subprocedure .
  ?subprocedure sp:hasAlertMessage ?caution .
  ?subprocedure sp:hasDescription ?subprocedureDescUri .
  ?subprocedureDescUri rdf:value ?subprocedureDesc .
  ?caution a <http://www.owl-ontologies.com/Ontology1184060740.owl#Class_122> .
  ?caution rdf:value ?cautionDescription .
  ?reagentNameUri <http://purl.obolibrary.org/obo/RO_0000056> ?subprocedure .
  ?reagentNameUri rdf:value ?reagentName .
} GROUP BY ?subprocedureDesc ?cautionDescription
```

## 21. Retrieve the provenance of the protocol titled “Scratch Wound Healing Assay”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0A%0D%0ASELECT+%3Fprovenance%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%22Scratch+Wound+Healing+Assay%22++.%0D%0A++%3Fprotocol+sp%3AhasProvenance+%3FprovenanceUri+.%0D%0A++%3FprovenanceUri+rdf%3Avalue+%3Fprovenance+.%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?provenance
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value "Scratch Wound Healing Assay"  .
  ?protocol sp:hasProvenance ?provenanceUri .
  ?provenanceUri rdf:value ?provenance .
}
```

## 22. Retrieve the specimen names that could be tested in the protocols titled “A simplified universal genomic DNA extraction protocol suitable for PCR” and “RNA Isolation from Synechocystis”
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0A%0D%0ASELECT+%3Ftitle%0D%0A%28group_concat%28distinct%28%3FspecimenName%29%3B+separator%3D%22+%2C+%22%29+as+%3FspecimenNames%29%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Fspecimens+.%0D%0A++%3Fspecimens+a+sp%3ASpecimenList+.%0D%0A++%3Fspecimens+ro%3Ahas_part+%3FspecimenNameUri+.%0D%0A++%3FspecimenNameUri+rdf%3Avalue+%3FspecimenName+.%0D%0A++FILTER%28%3Ftitle+%3D+%22A+simplified+universal+genomic+DNA+extraction+protocol+suitable+for+PCR%22+%7C%7C+%3Ftitle+%3D+%22RNA+Isolation+from+Synechocystis%22%29%0D%0A%7D+GROUP+BY+%3Ftitle&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>

SELECT ?title
(group_concat(distinct(?specimenName); separator=" , ") as ?specimenNames)
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?specimens .
  ?specimens a sp:SpecimenList .
  ?specimens ro:has_part ?specimenNameUri .
  ?specimenNameUri rdf:value ?specimenName .
  FILTER(?title = "A simplified universal genomic DNA extraction protocol suitable for PCR" || ?title = "RNA Isolation from Synechocystis")
} GROUP BY ?title
```


## 23. Retrieve the protocols and the list of reagents for documents authored by Yanling Chen.
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+IAO%3A+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FIAO_%3E%0D%0A%0D%0ASELECT+%3Ftitle+%28group_concat%28distinct%28%3FreagentName%29%3Bseparator%3D%22+%7C+%22%29+as+%3FreagentNames%29%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++%0D%0A++%3Fprotocol+ro%3Ahas_part+%3Fauthors+.%0D%0A++%3Fauthors+a+IAO%3A0000321+.%0D%0A++%3Fauthors+ro%3Ahas_part+%3FauthorNameUri+.%0D%0A++%3FauthorNameUri+rdf%3Avalue+%22Yanling+Chen%22+.%0D%0A%7D+GROUP+BY+%3Ftitle&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX IAO: <http://purl.obolibrary.org/obo/IAO_>

SELECT ?title (group_concat(distinct(?reagentName);separator=" | ") as ?reagentNames)
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagentNameUri rdf:value ?reagentName .
  
  ?protocol ro:has_part ?authors .
  ?authors a IAO:0000321 .
  ?authors ro:has_part ?authorNameUri .
  ?authorNameUri rdf:value "Yanling Chen" .
} GROUP BY ?title
```


## 24. Retrieve the protocols authored by Cristian Olaya and Wilmer Cuellar using Cassava (NCBITAXON:3983) as a sample 
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+IAO%3A+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FIAO_%3E%0D%0A%0D%0ASELECT+%3Ftitle+%28group_concat%28distinct%28%3FreagentName%29%3Bseparator%3D%22+%7C+%22%29+as+%3FprotocolReagents%29%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Fsamples+.%0D%0A++%3Fsamples+a+sp%3ASpecimenList.%0D%0A++%3Fsamples+ro%3Ahas_part+%3FsampleNameUri+.%0D%0A++%3Fsample+sp%3AhasName+%3FsampleNameUri+.%0D%0A++%3Fsample+owl%3AsameAs+%3Chttp%3A%2F%2Fpurl.bioontology.org%2Fontology%2FNCBITAXON%2F3983%3E+.%0D%0A++%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++%0D%0A++%3Fprotocol+ro%3Ahas_part+%3Fauthors+.%0D%0A++%3Fauthors+a+IAO%3A0000321+.%0D%0A++%3Fauthors+ro%3Ahas_part+%3FauthorNameUri1+.%0D%0A++%3FauthorNameUri1+rdf%3Avalue+%22Cristian+Olaya%22+.%0D%0A++%3Fauthors+ro%3Ahas_part+%3FauthorNameUri2+.%0D%0A++%3FauthorNameUri2+rdf%3Avalue+%22Wilmer+Cuellar%22+.%0D%0A%7D+GROUP+BY+%3Ftitle&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX IAO: <http://purl.obolibrary.org/obo/IAO_>

SELECT ?title (group_concat(distinct(?reagentName);separator=" | ") as ?protocolReagents)
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?samples .
  ?samples a sp:SpecimenList.
  ?samples ro:has_part ?sampleNameUri .
  ?sample sp:hasName ?sampleNameUri .
  ?sample owl:sameAs <http://purl.bioontology.org/ontology/NCBITAXON/3983> .
  
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagentNameUri rdf:value ?reagentName .
  
  ?protocol ro:has_part ?authors .
  ?authors a IAO:0000321 .
  ?authors ro:has_part ?authorNameUri1 .
  ?authorNameUri1 rdf:value "Cristian Olaya" .
  ?authors ro:has_part ?authorNameUri2 .
  ?authorNameUri2 rdf:value "Wilmer Cuellar" .
} GROUP BY ?title
```

## 25. Retrieve the common reagents across the protocols "[Bio101] Subcutaneous Injection of Tumor Cells" and "Scratch Wound Healing Assay"
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0APREFIX+IAO%3A+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FIAO_%3E%0D%0A%0D%0ASELECT+%3FcommonReagentName%0D%0AWHERE+%7B%0D%0A++%3Fprotocol1+sp%3AhasTitle+%3Ftitle_uri1+.%0D%0A++%3Ftitle_uri1+rdf%3Avalue+%22%5BBio101%5D+Subcutaneous+Injection+of+Tumor+Cells%22+.%0D%0A++%3Fprotocol1+sp%3AhasExperimentalInput+%3Freagents1+.%0D%0A++%3Freagents1+a+sp%3AReagentList+.%0D%0A++%3Freagents1+ro%3Ahas_part+%3FreagentNameUri1+.%0D%0A++%3FreagentNameUri1+rdf%3Avalue+%3FcommonReagentName+.%0D%0A+%0D%0A++%3Fprotocol2+sp%3AhasTitle+%3Ftitle_uri2+.%0D%0A++%3Ftitle_uri2+rdf%3Avalue+%22Scratch+Wound+Healing+Assay%22+.%0D%0A++%3Fprotocol2+sp%3AhasExperimentalInput+%3Freagents2+.%0D%0A++%3Freagents2+a+sp%3AReagentList+.%0D%0A++%3Freagents2+ro%3Ahas_part+%3FreagentNameUri2+.%0D%0A++%3FreagentNameUri2+rdf%3Avalue+%3FcommonReagentName+.%0D%0A%7D&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX IAO: <http://purl.obolibrary.org/obo/IAO_>

SELECT ?commonReagentName
WHERE {
  ?protocol1 sp:hasTitle ?title_uri1 .
  ?title_uri1 rdf:value "[Bio101] Subcutaneous Injection of Tumor Cells" .
  ?protocol1 sp:hasExperimentalInput ?reagents1 .
  ?reagents1 a sp:ReagentList .
  ?reagents1 ro:has_part ?reagentNameUri1 .
  ?reagentNameUri1 rdf:value ?commonReagentName .
 
  ?protocol2 sp:hasTitle ?title_uri2 .
  ?title_uri2 rdf:value "Scratch Wound Healing Assay" .
  ?protocol2 sp:hasExperimentalInput ?reagents2 .
  ?reagents2 a sp:ReagentList .
  ?reagents2 ro:has_part ?reagentNameUri2 .
  ?reagentNameUri2 rdf:value ?commonReagentName .
}
```

## 26. Retrieve the protocols in which Bromophenol blue is used and tell me about the application of Bromophenol blue
<a href="http://smartprotocols.linkeddata.es/sparql?default-graph-uri=&query=PREFIX+sp%3A+%3Chttp%3A%2F%2Fpurl.org%2Fnet%2FSMARTprotocol%23%3E%0D%0APREFIX+rdf%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0D%0APREFIX+ro%3A+%3Chttp%3A%2F%2Fwww.obofoundry.org%2Fro%2Fro.owl%23%3E%0D%0APREFIX+owl%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2002%2F07%2Fowl%23%3E%0D%0A%0D%0ASELECT+%3FreagentName+%3Fdesc+%28group_concat%28%3Ftitle%3B+separator%3D%22+%7C+%22%29+as+%3Fprotocols%29%0D%0AWHERE+%7B%0D%0A++%3Fprotocol+sp%3AhasTitle+%3Ftitle_uri+.%0D%0A++%3Ftitle_uri+rdf%3Avalue+%3Ftitle+.%0D%0A++%3Fprotocol+sp%3AhasExperimentalInput+%3Freagents+.%0D%0A++%3Freagents+a+sp%3AReagentList+.%0D%0A++%3Freagents+ro%3Ahas_part+%3FreagentNameUri+.%0D%0A++%3FreagentNameUri+rdf%3Avalue+%3FreagentName+.%0D%0A++%3Freagent+sp%3AhasName+%3FreagentNameUri+.%0D%0A++%3Freagent+owl%3AsameAs+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FCHEBI_59424%3E+.%0D%0A++%0D%0A++SERVICE+%3Chttp%3A%2F%2Fsparql.bioontology.org%2Fontologies%2Fsparql%2F%3Fapikey%3DINSERT+YOUR+BIOPORTAL+APIKEY+HERE%3E+%7B%0D%0A+++++++++++%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FCHEBI_59424%3E+%3Chttp%3A%2F%2Fpurl.obolibrary.org%2Fobo%2Fdef%3E+%3Fdesc+.%0D%0A++%7D%0D%0A%7D+GROUP+BY+%3FreagentName+%3Fdesc&should-sponge=&format=text%2Fhtml&timeout=0&debug=on" target="_blank">Execute it in the endpoint</a>  

```
PREFIX sp: <http://purl.org/net/SMARTprotocol#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX ro: <http://www.obofoundry.org/ro/ro.owl#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>

SELECT ?reagentName ?desc (group_concat(?title; separator=" | ") as ?protocols)
WHERE {
  ?protocol sp:hasTitle ?title_uri .
  ?title_uri rdf:value ?title .
  ?protocol sp:hasExperimentalInput ?reagents .
  ?reagents a sp:ReagentList .
  ?reagents ro:has_part ?reagentNameUri .
  ?reagentNameUri rdf:value ?reagentName .
  ?reagent sp:hasName ?reagentNameUri .
  ?reagent owl:sameAs <http://purl.obolibrary.org/obo/CHEBI_59424> .
  
  SERVICE <http://sparql.bioontology.org/ontologies/sparql/?apikey=INSERT YOUR BIOPORTAL APIKEY HERE> {
           <http://purl.obolibrary.org/obo/CHEBI_59424> <http://purl.obolibrary.org/obo/def> ?desc .
  }
} GROUP BY ?reagentName ?desc

```