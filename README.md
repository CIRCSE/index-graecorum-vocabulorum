# Index Graecorum Vocabulorum in Linguam Latinam	

Manually-corrected OCR of G.A. Saalfeld's list of 1,763 Latin loans from Ancient Greek (1874). This work was carried out as part of an internship at the [CIRCSE Research Centre](https://centridiricerca.unicatt.it/circse_index.html) in Milan, Italy, in the context of the [_LiLa: Linking Latin_](https://lila-erc.eu/) project.

- PDF of the _Index_: [indexgraecorvmvo00saal/page/n7/mode/2up](https://archive.org/details/indexgraecorvmvo00saal/page/n7/mode/2up)
- Dirty OCR of the _Index_: [indexgraecorvmvo00saal/indexgraecorvmvo00saal_djvu.txt](https://ia800300.us.archive.org/35/items/indexgraecorvmvo00saal/indexgraecorvmvo00saal_djvu.txt) 
- PDF of the extended edition of the _Index_, published in 1884: [tensaurusitalogr00saal/page/n3/mode/2up](https://archive.org/details/tensaurusitalogr00saal/page/n3/mode/2up)

## `igvll.txt` file structure

1. `lila_id`
2. `lemma_latin`, as recorded in the _Index_
3. `lemma_greek`, as recorded in the _Index_:
   - `certainty` indicates editorial uncertainty
   - `written_representation`, i.e. graphical variants of the same lemma
   - `lemma_variant`, i.e. alternative lemmas
   - `compound`, i.e. compound lemmas
<!--4. `lsj_exactMatch,lsj_broadMatch,lsj_relatedMatch`, where available. If empty, no LSJ CITE URN available. LSJ CITE URN: https://raw.githubusercontent.com/Eumaeus/cite_lsj_cex/master/lsj_index.txt-->

<!-- ## Ontology examples

<!--#### Lexical Entry (Latin)
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/LexicalEntry/abacus>
    a                     ontolex:LexicalEntry ;
    rdfs:label            "abacus" ;
    ontolex:canonicalForm <https://lila-erc.eu/data/id/lemma/86829> ;
    lemonEty:etymology    <http://lila-erc.eu/.../IGVLL/id/etymology/1> .
```
-->

<!--#### Etymon (Ancient Greek)
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/1>
    a                      lemonEty:Etymon ;
    rdfs:label             "ἄβαξ" ;
    lime:language          "grc" ;
    ontolex:canonicalForm  [ ontolex:writtenRep "ἄβαξ" ] ;
    skos:exactMatch  <urn:cite2:hmt:lsj.chicago_md:n51> .
```
-->

<!--#### Etymology
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymology/1>
    a                      crm:E89 , lemonEty:Etymology ;
    rdfs:label             "Etymology of: abacus" ;
    lemonEty:etymon        <http://lila-erc.eu/.../IGVLL/id/LexicalEntry/abacus> ,
                           <http://lila-erc.eu/.../IGVLL/id/etymon/1> ;
```
-->

<!--#### Etymology Link
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etylink/1>
    a                     lemonEty:EtyLink ;
    rdfs:label            "Etymology Link" ;
    lemonEty:etyLinkType  "borrowing" ;
    lemonEty:etySource    <http://lila-erc.eu/.../IGVLL/id/etymon/1> ;
    lemonEty:etyTarget    <http://lila-erc.eu/.../IGVLL/id/LexicalEntry/abacus> .
```


<!--#### Lemma variants: cyperum

<!--##### Etymon
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/4>
    a                      lemonEty:Etymon ;
    rdfs:label             "κύπειρον" ;
    lime:language          "grc" ;
    ontolex:canonicalForm  [ ontolex:writtenRep "κύπειρον" ] ;
    skos:exactMatch  <urn:cite2:hmt:lsj.chicago_md:n60988> ;
    lemonEty:cognate      <http://lila-erc.eu/.../IGVLL/id/etymon/5> .
```
-->

<!--##### Cognate of Etymon
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/5>
    a                      lemonEty:Etymon, lemonEty:Cognate ;
    rdfs:label             "κύπειρος" ;
    lime:language          "grc" ;
    ontolex:canonicalForm  [ ontolex:writtenRep "κύπειρος" ] ;
    skos:exactMatch  <urn:cite2:hmt:lsj.chicago_md:n91854> .
```
-->

<!--##### Belief Value: aura
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/belief/1>
    a                     crminf:I2 ;
    rdfs:label            "Belief that the etymology of aura is uncertain" ;
    crminf:J4             <http://lila-erc.eu/.../IGVLL/id/etymology/2> ;
    crminf:J5             [ a crminf:I6 ; ov:confidence 0.5 ] .
```
-->


<!--#### Compounds: authepsa

<!--##### Lexical Entry
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/LexicalEntry/authepsa>
    a                     ontolex:LexicalEntry ;
    rdfs:label            "authepsa" ;
    ontolex:canonicalForm <https://lila-erc.eu/data/id/lemma/90834> ;
    lemonEty:etymology    <http://lila-erc.eu/.../IGVLL/id/etymology/5> .
```
-->

<!--##### Ancient Greek Compound
```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/6>
    a                      lemonEty:Etymon ;
    decomp:subterm         <http://lila-erc.eu/.../IGVLL/id/etymon/7> ,
                           <http://lila-erc.eu/.../IGVLL/id/etymon/8> .
```
-->

## Credits

- **Creators**: Greta Franzini, Federica Zampedri, Marco Passarotti
- **Contributors**: Francesco Mambrini, Giovanni Moretti

The _LiLa: Linking Latin_ project has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme – Grant Agreement No. 769994.

<!--### Citation-->
<!--To cite this data-set, you can adapt the following:-->
<!--Franzini, G., Zampedri, F., Passarotti, M. (2020) <em>Index Graecorum Vocabulorum in Linguam Latinam: Manually-corrected OCR of G.A. Saalfeld's list of 1,763 Latin loans from Ancient Greek (1874), mapped to the</em> LiLa: Linking Latin <em>lemma bank and the</em> Liddell-Scott Jones CITE Application. DOI: doi here-->


## Copyright

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

## Citation

[![DOI](https://zenodo.org/badge/271791451.svg)](https://zenodo.org/badge/latestdoi/271791451)
