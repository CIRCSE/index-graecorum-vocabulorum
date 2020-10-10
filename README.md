# Index Graecorum Vocabulorum in Linguam Latinam	

Manually-corrected OCR of G.A. Saalfeld's list of 1,763 Latin loans from Ancient Greek (1874). This work was carried out as part of an internship at the [CIRCSE Research Centre](https://centridiricerca.unicatt.it/circse_index.html) in Milan, Italy, in the context of the [_LiLa: Linking Latin_](https://lila-erc.eu/) project.

- PDF of the _Index_: [indexgraecorvmvo00saal/page/n7/mode/2up](https://archive.org/details/indexgraecorvmvo00saal/page/n7/mode/2up)
- Dirty OCR of the _Index_: [indexgraecorvmvo00saal/indexgraecorvmvo00saal_djvu.txt](https://ia800300.us.archive.org/35/items/indexgraecorvmvo00saal/indexgraecorvmvo00saal_djvu.txt) 
- PDF of the extended edition of the _Index_, published in 1884: [tensaurusitalogr00saal/page/n3/mode/2up](https://archive.org/details/tensaurusitalogr00saal/page/n3/mode/2up)

## `IGVLL.csv` file

1. `lila_id`
2. `lemma_latin`, as recorded in the _Index_
3. `lemma_greek`, as recorded in the _Index_:
4. `certainty` indicates editorial uncertainty on Greek provenance
5. `written_representation`, i.e. graphical variants of the Greek lemma(s)
6. `lemma_variant`, i.e. alternative Greek lemma(s)
7. `compound`, i.e. compound Greek lemmas
8. `lsj_exactMatch`: where available, URN of the corresponding Ancient Greek lemma in the [LSJ CITE APP](https://raw.githubusercontent.com/Eumaeus/cite_lsj_cex/master/lsj_index.txt)
9. `lsj_broadMatch`: failing an `lsj_exactMatch`, where available, the URN of the nearest match in the LSJ CITE APP (e.g. φυσική vs. φυσικός)
10. `lsj_relatedMatch`: failing an `lsj_exactMatch` and an `lsj_broadMatch,` where available, the URN of a related lemma in the LSJ CITE APP (e.g. ἐντεροκηλικός vs. ἐντεροκήλη)

## `IGVLL.ttl` Turtle file


### Example entry in the Terse RDF Triple Language (Turtle) syntax: `abacus`

```
<http://lila-erc.eu/data/lexicalResources/IGVLL/id/LexicalEntry/abacus> a ontolex:LexicalEntry;
  lemonEty:etymology <http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymology/1>;
  <http://www.w3.org/2000/01/rdf-schema#label> "abacus";
  ontolex:canonicalForm <http://lila-erc.eu/data/id/lemma/86829> .

<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/1> a lemonEty:Etymon;
  <http://www.w3.org/2000/01/rdf-schema#label> "ἄβαξ";
  skos:exactMatch <urn:cite2:hmt:lsj.chicago_md:n51>;
  lime:language "grc";
  ontolex:canonicalForm [ ontolex:writtenRep "ἄβαξ"  ] .

<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymology/1> a lemonEty:Etymology,
    crm:E89;
  lemonEty:etymon <http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/1>;
  lemonEty:hasEtyLink <http://lila-erc.eu/data/lexicalResources/IGVLL/id/etylink/1>;
  <http://www.w3.org/2000/01/rdf-schema#label> "Etymology of: abacus" .

<http://lila-erc.eu/data/lexicalResources/IGVLL/id/etylink/1> a lemonEty:EtyLink;
  lemonEty:etyLinkType "borrowing";
  lemonEty:etySource <http://lila-erc.eu/data/lexicalResources/IGVLL/id/etymon/1>;
  lemonEty:etyTarget <http://lila-erc.eu/data/lexicalResources/IGVLL/id/LexicalEntry/abacus>;
  <http://www.w3.org/2000/01/rdf-schema#label> "Etymology Link" .
```


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
