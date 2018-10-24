# KnowledgePearls:  Provenance-based Visualization Retrieval

![Vega Gapminder](https://raw.githubusercontent.com/Caleydo/knowledge-pearls/assets/vega-gapminder.png)

[Link to the Vega Gapminder demo with the recorded provenance graph shown in the Figure above.](https://vega-gapminder.caleydoapp.org/#clue_graph=persistentWsL5Fis&clue_state=40)

Storing analytical provenance generates a knowledge base with a large potential for recalling previous results and guiding users in future analyses. However, without extensive manual creation of meta information and annotations by the users, search and retrieval of analysis states can become tedious.

We present KnowledgePearls, a solution for efficient retrieval of analysis states that are structured as provenance graphs containing automatically recorded user interactions and visualizations. As a core component, we describe a visual interface for querying and exploring analysis states based on their similarity to a partial definition of a requested analysis state. Depending on the use case, this definition may be provided explicitly by the user by formulating a search query or inferred from given reference states. We explain our approach using the example of efficient retrieval of demographic analyses by Hans Rosling and discuss our implementation for a fast look-up of previous states. Our approach is independent of the underlying visualization framework. We discuss the applicability for visualizations which are based on the declarative grammar Vega and we use a Vega-based implementation of Gapminder as guiding example. We additionally present a biomedical case study to illustrate how KnowledgePearls facilitates the exploration process by recalling states from earlier analyses.

## Publication

You can find the publication on the [Caleydo](http://caleydo.org/publications/2018_vast_knowledge-pearls/) website.

```
Holger Stitz, Samuel Gratzl, Harald Piringer, Thomas Zichner, Marc Streit
KnowledgePearls: Provenance-Based Visualization Retrieval
IEEE Transactions on Visualization and Computer Graphics (VAST '18), to appear, doi:10.1109/TVCG.2017.2745298, 2018. 
```


## Demos

* [Vega Gapminder](https://vega-gapminder.caleydoapp.org) (with an empty provenance graph)
* [Vega Gapminder demo with a recorded provenance graph ready for retrieval](https://vega-gapminder.caleydoapp.org/#clue_graph=persistentWsL5Fis&clue_state=40)
* [Ordino](https://ordino-retrieval.caleydoapp.org) (with an empty provenance graph)


## Installation

### Prerequisits

* [Docker](https://www.docker.com/)
* [Node/npm](http://nodejs.org/)
* [Phovea Generator](https://github.com/phovea/generator-phovea/)

### Vega Gapminder

```
yo phovea:setup-workspace Caleydo/vega_clue_product
docker-compose up -d
npm start
```

### Ordino

```
yo phovea:setup-workspace Caleydo/ordino_product -b provenance_retrieval
docker-compose up -d
npm start
```


## Source Code

* [Vega Gapminder](https://github.com/Caleydo/vega_clue)


