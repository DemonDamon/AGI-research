# 09_GraphRAG Paper

**原始链接**: https://arxiv.org/abs/2404.16130

---

# [2404.16130] From Local to Global: A Graph RAG Approach to Query-Focused Summarization

原文链接: https://arxiv.org/abs/2404.16130

# Computer Science > Computation and Language

**arXiv:2404.16130** (cs)

[Submitted on 24 Apr 2024 ([v1](https://arxiv.org/abs/2404.16130v1)), last revised 19 Feb 2025 (this version, v2)]

# Title:From Local to Global: A Graph RAG Approach to Query-Focused Summarization

Authors:[Darren Edge](https://arxiv.org/search/cs?searchtype=author&query=Edge,+D), [Ha Trinh](https://arxiv.org/search/cs?searchtype=author&query=Trinh,+H), [Newman Cheng](https://arxiv.org/search/cs?searchtype=author&query=Cheng,+N), [Joshua Bradley](https://arxiv.org/search/cs?searchtype=author&query=Bradley,+J), [Alex Chao](https://arxiv.org/search/cs?searchtype=author&query=Chao,+A), [Apurva Mody](https://arxiv.org/search/cs?searchtype=author&query=Mody,+A), [Steven Truitt](https://arxiv.org/search/cs?searchtype=author&query=Truitt,+S), [Dasha Metropolitansky](https://arxiv.org/search/cs?searchtype=author&query=Metropolitansky,+D), [Robert Osazuwa Ness](https://arxiv.org/search/cs?searchtype=author&query=Ness,+R+O), [Jonathan Larson](https://arxiv.org/search/cs?searchtype=author&query=Larson,+J)

View a PDF of the paper titled From Local to Global: A Graph RAG Approach to Query-Focused Summarization, by Darren Edge and 9 other authors

[View PDF](/pdf/2404.16130)
[HTML (experimental)](https://arxiv.org/html/2404.16130v2)
> Abstract:The use of retrieval-augmented generation (RAG) to retrieve relevant information from an external knowledge source enables large language models (LLMs) to answer questions over private and/or previously unseen document collections. However, RAG fails on global questions directed at an entire text corpus, such as "What are the main themes in the dataset?", since this is inherently a query-focused summarization (QFS) task, rather than an explicit retrieval task. Prior QFS methods, meanwhile, do not scale to the quantities of text indexed by typical RAG systems. To combine the strengths of these contrasting methods, we propose GraphRAG, a graph-based approach to question answering over private text corpora that scales with both the generality of user questions and the quantity of source text. Our approach uses an LLM to build a graph index in two stages: first, to derive an entity knowledge graph from the source documents, then to pregenerate community summaries for all groups of closely related entities. Given a question, each community summary is used to generate a partial response, before all partial responses are again summarized in a final response to the user. For a class of global sensemaking questions over datasets in the 1 million token range, we show that GraphRAG leads to substantial improvements over a conventional RAG baseline for both the comprehensiveness and diversity of generated answers.

|  |  |
| --- | --- |
| Subjects: | Computation and Language (cs.CL); Artificial Intelligence (cs.AI); Information Retrieval (cs.IR) |
| ACM classes: | H.3.3; I.2.7 |
| Cite as: | [arXiv:2404.16130](https://arxiv.org/abs/2404.16130) [cs.CL] |
|  | (or  [arXiv:2404.16130v2](https://arxiv.org/abs/2404.16130v2) [cs.CL] for this version) |
|  | <https://doi.org/10.48550/arXiv.2404.16130> Focus to learn more  arXiv-issued DOI via DataCite |

## Submission history

From: Darren Edge [[view email](/show-email/99103aef/2404.16130)]   
 **[[v1]](/abs/2404.16130v1)**
Wed, 24 Apr 2024 18:38:11 UTC (6,306 KB)  
**[v2]**
Wed, 19 Feb 2025 10:49:41 UTC (6,322 KB)

Full-text links:

## Access Paper:

View a PDF of the paper titled From Local to Global: A Graph RAG Approach to Query-Focused Summarization, by Darren Edge and 9 other authors

* [View PDF](/pdf/2404.16130)
* [HTML (experimental)](https://arxiv.org/html/2404.16130v2)
* [TeX Source](/src/2404.16130)

[![license icon](images/5e2067e78de5c37cc40951f64c88226b.png)
view license](http://creativecommons.org/licenses/by/4.0/ "Rights to this article")

Current browse context:

cs.CL

[< prev](/prevnext?id=2404.16130&function=prev&context=cs.CL "previous in cs.CL (accesskey p)")
  |   
[next >](/prevnext?id=2404.16130&function=next&context=cs.CL "next in cs.CL (accesskey n)")

[new](/list/cs.CL/new)
 | 
[recent](/list/cs.CL/recent)
 | [2024-04](/list/cs.CL/2024-04)

Change to browse by:

[cs](/abs/2404.16130?context=cs)  
[cs.AI](/abs/2404.16130?context=cs.AI)  
[cs.IR](/abs/2404.16130?context=cs.IR)

### References & Citations

* [NASA ADS](https://ui.adsabs.harvard.edu/abs/arXiv:2404.16130)
* [Google Scholar](https://scholar.google.com/scholar_lookup?arxiv_id=2404.16130)
* [Semantic Scholar](https://api.semanticscholar.org/arXiv:2404.16130)

export BibTeX citation
Loading...

## BibTeX formatted citation

×

loading...

Data provided by:

### Bookmark

[![BibSonomy logo](images/beeafe67a38fcaeb5dd2ebdbd21eeb1b.png)](images/3edb3542d5e3dd93393f036f43e24013.jpg)
[![Reddit logo](images/81596774e6fbaf50c3fb294d1f5232cc.png)](images/99cce065ba783c97e5299bea243ba1ac.jpg)



Bibliographic Tools

# Bibliographic and Citation Tools

Bibliographic Explorer Toggle

Bibliographic Explorer *([What is the Explorer?](https://info.arxiv.org/labs/showcase.html#arxiv-bibliographic-explorer))*

Connected Papers Toggle

Connected Papers *([What is Connected Papers?](https://www.connectedpapers.com/about))*

Litmaps Toggle

Litmaps *([What is Litmaps?](https://www.litmaps.co/))*

scite.ai Toggle

scite Smart Citations *([What are Smart Citations?](https://www.scite.ai/))*

Code, Data, Media

# Code, Data and Media Associated with this Article

alphaXiv Toggle

alphaXiv *([What is alphaXiv?](https://alphaxiv.org/))*

Links to Code Toggle

CatalyzeX Code Finder for Papers *([What is CatalyzeX?](https://www.catalyzex.com))*

DagsHub Toggle

DagsHub *([What is DagsHub?](https://dagshub.com/))*

GotitPub Toggle

Gotit.pub *([What is GotitPub?](http://gotit.pub/faq))*

Huggingface Toggle

Hugging Face *([What is Huggingface?](https://huggingface.co/huggingface))*

Links to Code Toggle

Papers with Code *([What is Papers with Code?](https://paperswithcode.com/))*

ScienceCast Toggle

ScienceCast *([What is ScienceCast?](https://sciencecast.org/welcome))*

Demos

# Demos

Replicate Toggle

Replicate *([What is Replicate?](https://replicate.com/docs/arxiv/about))*

Spaces Toggle

Hugging Face Spaces *([What is Spaces?](https://huggingface.co/docs/hub/spaces))*

Spaces Toggle

TXYZ.AI *([What is TXYZ.AI?](https://txyz.ai))*

Related Papers

# Recommenders and Search Tools

Link to Influence Flower

Influence Flower *([What are Influence Flowers?](https://influencemap.cmlab.dev/))*

Core recommender toggle

CORE Recommender *([What is CORE?](https://core.ac.uk/services/recommender))*

* Author
* Venue
* Institution
* Topic


About arXivLabs

# arXivLabs: experimental projects with community collaborators

arXivLabs is a framework that allows collaborators to develop and share new arXiv features directly on our website.

Both individuals and organizations that work with arXivLabs have embraced and accepted our values of openness, community, excellence, and user data privacy. arXiv is committed to these values and only works with partners that adhere to them.

Have an idea for a project that will add value for arXiv's community? [**Learn more about arXivLabs**](https://info.arxiv.org/labs/index.html).

[Which authors of this paper are endorsers?](/auth/show-endorsers/2404.16130) |
[Disable MathJax](javascript:setMathjaxCookie()) ([What is MathJax?](https://info.arxiv.org/help/mathjax.html))