DBpedia_PageRank_Scores
================

##Source Dataset


DBpedia_PageLinks_Cleaned Dataset (3.9) is used to compute Pagerank. More details about DBpedia_PageLinks_Cleaned Dataset and how it is created can be found [here](http://semanticmultimedia.org/node/6).


##Implementation

JUNG — the Java Universal Network/Graph Framework is used to compute pagerank. JUNG is a software library that provides a common and extendible language for the modeling, analysis, and visualization of data that can be represented as a graph or network. 

You can get the soucre code at [JUNG PageRank Implementation](https://github.com/dineshreddykdp/JungGraphMeasures)

Parameters used while computing pagerank

```
PageRank damping factor: 0.85 //The probability at any step, that the person will continue
PageRank no of iterations: 100 //Number of iterations used before terminating
PageRank Tolerance: 0 //Minimum change from one step to the next
Alpha: 0.15 //Random jump probability, the probability of taking a random jump to an arbitrary vertex
```
##Citation

If you are using this dataset please cite as:

```
{dbpedia-graphmeasures,
  Author = {Dinesh Reddy},
  Title = {DBpedia GraphMeasures},
  Location = {http://semanticmultimedia.org/node/6},
  Resource type = {dataset},
  Publisher = {Hasso Plattner Institute},
  Publication date = {July 2014},
}
```
##Details of the datasets


Details | English | German
------- | ------- | ------
Number of Triples(resources) | 4984633 | 1689764
File Memory | 75.3 MB | 25 MB
Format | Turtle | Turtle



##Schema 


Top 5 resources with high pagerank from DBpedia_page_links_cleaned_English Dataset

```
<http://dbpedia.org/resource/Category:Living_people> <http://dbpedia.org/ontology/wikiPageRank> "0.002395068441893186"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/United_States> <http://dbpedia.org/ontology/wikiPageRank> "0.0022332560183101467"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/France> <http://dbpedia.org/ontology/wikiPageRank> "9.266472266155261E-4"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/List_of_sovereign_states> <http://dbpedia.org/ontology/wikiPageRank> "8.753350014750164E-4"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/Animal> <http://dbpedia.org/ontology/wikiPageRank> "8.645187491107416E-4"^^<http://www.w3.org/2001/XMLSchema#float> .
```

Top 5 resources with high pagerank from DBpedia_page_links_cleaned_German Dataset

```
<http://de.dbpedia.org/resource/Kategorie:Mann> <http://dbpedia.org/ontology/wikiPageRank> "0.004087672881729741"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/Vereinigte_Staaten> <http://dbpedia.org/ontology/wikiPageRank> "0.001758150354139443"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/Deutschland> <http://dbpedia.org/ontology/wikiPageRank> "0.001419473129061212"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/Kategorie:Deutscher> <http://dbpedia.org/ontology/wikiPageRank> "0.0012921635322098008"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/Frankreich> <http://dbpedia.org/ontology/wikiPageRank> "0.001063181276253678"^^<http://www.w3.org/2001/XMLSchema#float> .
```
