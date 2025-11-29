# Machine Learning in Materials Discovery

**来源**: [https://www.annualreviews.org/content/journals/10.1146/annurev-matsci-090319-010954](https://www.annualreviews.org/content/journals/10.1146/annurev-matsci-090319-010954)

---

# Machine Learning in Materials Discovery: Confirmed Predictions and Their Underlying Approaches | Annual Reviews

原文链接: https://www.annualreviews.org/content/journals/10.1146/annurev-matsci-090319-010954

### [Annual Review of Materials Research](/content/journals/matsci)

[#### Volume 50, 2020](/content/journals/matsci/50/1)

#### Review Article

#### Free

# Machine Learning in Materials Discovery: Confirmed Predictions and Their Underlying Approaches

* [James E. Saal](/search?value1=James+E.+Saal&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)1, [Anton O. Oliynyk](/search?value1=Anton+O.+Oliynyk&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)1 and [Bryce Meredig](/search?value1=Bryce+Meredig&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)1
* [View Affiliations



  Hide Affiliations](#)

  1Citrine Informatics, Redwood City, California 94063, USA; email: [bryce@citrine.io](mailto:bryce@citrine.io)


  2Department of Chemistry and Biochemistry, Manhattan College, Riverdale, New York 10471, USA
* Vol. 50:49-69
  (Volume publication date July 2020)
  <https://doi.org/10.1146/annurev-matsci-090319-010954>
* First published as a Review in Advance on
  May 18, 2020
* Copyright © 2020 by Annual Reviews. All rights reserved

### Abstract

The rapidly growing interest in machine learning (ML) for materials discovery has resulted in a large body of published work. However, only a small fraction of these publications includes confirmation of ML predictions, either via experiment or via physics-based simulations. In this review, we first identify the core components common to materials informatics discovery pipelines, such as training data, choice of ML algorithm, and measurement of model performance. Then we discuss some prominent examples of validated ML-driven materials discovery across a wide variety of materials classes, with special attention to methodological considerations and advances. Across these case studies, we identify several common themes, such as the use of domain knowledge to inform ML models.



**Keyword(s):**
[machine learning](/search?value1=%22machine+learning%22&option1=pub_keyword "machine learning"), [materials discovery](/search?value1=%22materials+discovery%22&option1=pub_keyword "materials discovery"), [materials informatics](/search?value1=%22materials+informatics%22&option1=pub_keyword "materials informatics")

![Loading](/images/jp/spinner.gif)

Article metrics loading...

/content/journals/10.1146/annurev-matsci-090319-010954

2020-07-01

2025-11-29

[Download as PowerPoint](#)


* ISSN: 1531-7331, Online ISSN: 1545-4118
* DOI: http://dx.doi.org/10.1146/annurev-matsci-090319-010954
* Volume 50, Issue 1, pages 49-69
* Copyright © 2020 by Annual Reviews. All rights reserved

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

# Machine Learning in Materials Discovery: Confirmed Predictions and Their Underlying Approaches

; ;

1Citrine Informatics, Redwood City, California 94063, USA; email: [bryce@citrine.io](mailto:bryce@citrine.io)
2Department of Chemistry and Biochemistry, Manhattan College, Riverdale, New York 10471, USA

ABSTRACT

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

The rapidly growing interest in machine learning (ML) for materials discovery has resulted in a large body of published work. However, only a small fraction of these publications includes confirmation of ML predictions, either via experiment or via physics-based simulations. In this review, we first identify the core components common to materials informatics discovery pipelines, such as training data, choice of ML algorithm, and measurement of model performance. Then we discuss some prominent examples of validated ML-driven materials discovery across a wide variety of materials classes, with special attention to methodological considerations and advances. Across these case studies, we identify several common themes, such as the use of domain knowledge to inform ML models.

Keywords

* [machine learning](/search?option1=pub_keyword&value1="machine learning"),
* [materials discovery](/search?option1=pub_keyword&value1="materials discovery"),
* [materials informatics](/search?option1=pub_keyword&value1="materials informatics")

1.  INTRODUCTION

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

Over the past decade, machine learning (ML) has emerged as a powerful tool to accelerate materials development ([1](#right-ref-B1 B2 B3 B4)–[5](#right-ref-B5)). Academic, government, and commercial entities are broadly deploying ML in service of materials discovery. Publication activity in ML for materials is growing exponentially even as a fraction of all materials research ([Figure 1](#f1)). Despite an increasing body of literature on data-driven materials research, which we refer to as materials informatics, only a fraction of published studies culminate in predictions that are subsequently validated by an experiment, either in the laboratory or as a “virtual” experiment via physics-based simulation. A trained ML model is merely a means to an end, and the utility of materials informatics is fully realized only when ML predictions are confirmed. In this review, we (a) describe the key components of a materials informatics discovery pipeline; (b) highlight recent works that describe validation of materials informatics predictions, as summarized in [Table 1](#t1); and (c) note some materials discovery–specific considerations for ML. We begin by describing a typical materials informatics pipeline in more detail.

Figure 1 
Share of materials and chemistry publications referencing machine learning (ML) as a function of time. The data are normalized to account for the overall exponential growth ([6](#right-ref-B6)) in scientific publications over time, illustrating the relative growth of ML-related work.

[![
                  Figure 1 
               ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/ab4c1aab85e59f52d8647cfd34a7066a.png)

Figure 1 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f1.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f1.ppt?mimeType=application/vnd.ms-powerpoint)

##### Table 1

Summary of validated machine learning (ML) predictions

[Toggle display:
Table 1](#) [Open
Table 1 
fullscreen](/content/table/10.1146/annurev-matsci-090319-010954.t1?fmt=ahah&fullscreen=true&lang=en)

| Reference | Materials class | Application | Predicted properties | Initial training data set | ML algorithm | Design space | Number of candidates evaluated | Yeara |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [70](#right-ref-B70) | Inorganic ternary solids (AxByCz) | Stable composition prediction | Formation energy | 15,000 density functional theory (DFT) calculations | Random forest | 1.6 million enumerated compositions | Nine DFT calculations | 2013 |
| [64](#right-ref-B64) | Molecules | Organic light-emitting diodes | Several underlying properties contributing to external quantum efficiency (EQE) | DFT calculations on 40,000 randomly selected candidates | Neural network | 1.6 million molecules constructed from fragments | Four experiments | 2015 |
| [90](#right-ref-B90) | Polymers | Dielectrics | Electronic dielectric constant, ionic dielectric constant, and band gap | Newly generated DFT data (284 records) | Kernel ridge regression and genetic algorithm | ∼156,000 enumerated four-, six-, and eight-block polymers | 28 DFT calculations | 2015 |
| [78](#right-ref-B78) | Organically templated metal oxides | Hydrothermal synthesis | Reaction success | Labeled reactions from internal data set (3,955 records) | Support vector machine | 1,680 commercially available diamines | 34 experiments | 2015 |
| [91](#right-ref-B91) | Inorganic binary solids (AB) | Structure discovery | Stability | Pearson's Crystal Data (PCD) database ([92](#right-ref-B92)) (706 records) | Support vector machine | 2,926 possible binary combinations | One experiment | 2016 |
| [65](#right-ref-B65) | Inorganic ternary solids (AB2C Heusler) | Structure discovery | Stability | PCD ([92](#right-ref-B92)) (1,948 records) | Random forest | >400,000 AB2C compositions | 21 experiments | 2016 |
| [68](#right-ref-B68) | Metal alloys | Shape memory alloys | Endothermic peak temperature | Newly synthesized alloys (53 records) | Polynomial regression | 1,652,470 compositions | One experiment | 2016 |
| [19](#right-ref-B19) | Perovskites | Ferroelectric | Ferroelectric Curie temperature and perovskite stability | Literature review (167 stability and 117 Curie temperature records) | Support vector classifier and linear regression | 61,506 enumerated compositions | 10 experiments | 2017 |
| [93](#right-ref-B93) | Inorganic ternary solids (ABC) | Structure discovery | Polymorphism | PCD ([92](#right-ref-B92)) (1,556 records) | Support vector machine | 98,769 ABC compositions | One experiment | 2017 |
| [7](#right-ref-B7) | Bulk metallic glasses | Structural applications | Glass formability | Landolt–Börnstein ([79](#right-ref-B79)) (6,780 records) | Random forest | Enumerated grids in 2,024 ternary systems | Four experiments | 2017 |
| [94](#right-ref-B94) | Ternary ionic solids (AaBbXx) | Structure discovery | Stability | Inorganic Crystal Structure Database (ICSD) ([95](#right-ref-B95)) | Tucker decomposition recommender system | 7,405,200 enumerated compositions | 27 DFT calculations | 2017 |
| [77](#right-ref-B77) | Metal–organic frameworks (MOFs) | Hydrogen storage | Hydrogen-deliverable capacity | Grand canonical Monte Carlo simulations (1,000 records) | Least absolute shrinkage and selection operator (LASSO) | 54,776 MOF structures from Cambridge Structural Database (CSD) ([9](#right-ref-B9)) | One experiment | 2018 |
| [63](#right-ref-B63) | Small molecules | Organic light- emitting diodes | Max light-absorbing wavelengths; triplet (T1) energy levels | Random sample from PubChem ([12](#right-ref-B12)) (50,000 records) | Deep neural network | 40,000 randomly generated simplified molecular-input line-entry system (SMILES) strings | Three experiments | 2018 |
| [96](#right-ref-B96) | Hybrid organic–inorganic perovskites (ABX3) | Photovoltaics | Band gap | Literature review (212 records) | Gradient boosting regression | 5,158 enumerated compositions | Six DFT calculations | 2018 |
| [31](#right-ref-B31) | Inorganic solids | Superhard materials | Bulk modulus and shear modulus | Materials Project ([28](#right-ref-B28)) (3,248 records) | Support vector machine | 118,287 compounds from PCD ([92](#right-ref-B92)) | Two experiments | 2018 |
| [75](#right-ref-B75) | Polymers | Cement plasticizer | Slump | Commercial data (seven records) | LASSO regression | Maximization of analytical expression for slump | One experiment | 2018 |
| [20](#right-ref-B20) | Ni-rich cathode materials (LiNixCo1 − x − y-Mn1 − x − y − zO2) | Batteries | Initial capacity, cycle life, and amount of residual Li | Literature review (330 records) | Extremely randomized tree and adaptive boosting | 50,000 randomly generated candidate syntheses | Five experiments | 2018 |
| [17](#right-ref-B17) | High-entropy alloys | Structural applications | Hardness | Literature review (82 records) | Canonical correlation analysis and genetic algorithm | 4.6 billion enumerated compositions | Seven experiments | 2018 |
| [80](#right-ref-B80) | Layered semiconductor metamaterials | Thermal radiator | Figure of merit from emissivity spectra | Iterative Bayesian optimization on 42,000 groups of structures | Gaussian process regression | >8 billion candidates | Three experiments | 2018 |
| [97](#right-ref-B97) | Polymers | Thermoplastics | Thermal conductivity (λ), several other properties | PoLyInfo ([98](#right-ref-B98)), QM9 ([99](#right-ref-B99)) (38,310 total properties; only 28 λ values) | Neural networks | Monte Carlo generative model (iqspr) | Three experiments | 2018 |
| [32](#right-ref-B32) | Inorganic phosphor host materials | Solid-state lighting | Debye temperature and band gap | Materials Project ([28](#right-ref-B28)) (2,610 records) | Support vector machine | >300,000 compounds from PCD ([92](#right-ref-B92)) | One experiment | 2018 |
| [82](#right-ref-B82) | Li-containing inorganic solids | Li-ion battery electrolytes | Ionic conductivity | Literature review and ICSD ([95](#right-ref-B95)) (40 records) | Logistic regression | 12,831 compounds from Materials Project ([28](#right-ref-B28)) | Four DFT calculations | 2019 |
| [22](#right-ref-B22) | High-entropy alloys (AlxCoyCrz-CuuFevNiw) | Structural applications | Hardness | Literature review and new experimental data (155 records) | Support vector machine | 1,895,147 compositions | 42 experiments | 2019 |

aYear the work was submitted for publication.

2.  THE MATERIALS INFORMATICS DISCOVERY PIPELINE

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

In this section, we discuss critical components of a materials informatics pipeline common to validated ML studies. These standard steps are summarized in the generalized pipeline of [Figure 2](#f2). The pipeline begins with establishing a materials data set for training, as well as a set of materials descriptors to extend the data with available physical information. This data set is then used to train an ML model, which is used to make a prediction of novel materials for validation.

Figure 2 
Schematic of a materials informatics discovery pipeline. The pipeline begins with input property data, which require a descriptor (i.e., vector) representation suitable for machine learning (ML). Model training and refinement comprise an iterative process, resulting in a model with known predictive performance that may be used to evaluate candidate materials. Data gathered from experiments or simulations should be used to further improve models, as described by Ren et al. ([7](#right-ref-B7)).

[![
                  Figure 2 
               ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/d561dcbcada57b7731a02efd43933b74.png)

Figure 2 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f2.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f2.ppt?mimeType=application/vnd.ms-powerpoint)

2.1.  
Training Data

Data of sufficient quality and quantity are an essential prerequisite for the successful application of ML methods to materials problems. Large companies in the technology industry, such as Google, Facebook, and Amazon, are able to train ML models on up to 1011 examples ([8](#right-ref-B8)). However, data are far more scarce in materials science, and data sets for materials discovery typically include 101–104 training examples, as seen in [Table 1](#t1).

Training data quality is associated with reliability and consistency. Reliability issues can result from unreported sources of variance (e.g., poorly calibrated or aged instruments) or human factors (e.g., typos that arise during manual data entry). Data consistency is related to the method that was used to generate the data. Inconsistency can be experimental (for example, thermal conductivity can be measured with different techniques, giving slightly different results) or computational (different simulation input choices can give different results).

2.1.1.  
Challenges in training data aggregation.

The source of training data for each materials problem must be considered on a case-by-case basis due to the lack of a centralized, homogeneous database of all materials measurements. Such authoritative databases are more common in the biological and pharmaceutical sciences; examples include the Cambridge Crystal Structure Database ([9](#right-ref-B9)), ChemBank ([10](#right-ref-B10)), GenBank ([11](#right-ref-B11)), and PubChem ([12](#right-ref-B12)). The materials science community has fewer data resources, although the Materials Data Facility ([13](#right-ref-B13)), the Novel Materials Discovery (NOMAD) Repository ([14](#right-ref-B14)), and Open Citrination ([15](#right-ref-B15)) have emerged to provide free-of-charge materials data services to the research community. However, for most materials problems, relevant experimental data are scattered across publications in the literature ([16](#right-ref-B16)), requiring researchers to manually extract and structure training data sets ([17](#right-ref-B17 B18 B19 B20 B21)–[22](#right-ref-B22)). While manually constructed data sets are highly time and resource intensive to build, they benefit from expert curation, which can be essential to providing the context needed for successful ML models.

2.1.2.  
Density functional theory as a source of training data.

Among successful materials informatics use cases, density functional theory (DFT) ([23](#right-ref-B23), [24](#right-ref-B24)) is a widely used source of training data and descriptors. DFT, as a means of generating large-scale materials data, has become more accessible over time ([25](#right-ref-B25), [26](#right-ref-B26)) as computational power has increased and the software has improved. The construction of high-throughput DFT (HT-DFT) databases ([27](#right-ref-B27 B28)–[29](#right-ref-B29)) has been a key contributor to many early informatics successes ([30](#right-ref-B30)). Advancing beyond relatively simple calculations of thermodynamic stability, more computationally costly HT-DFT data sets are enabling data-driven solutions to materials problems, such as DFT-calculated elastic tensors to predict superhard materials ([31](#right-ref-B31)) and discovery of novel phosphors for solid-state lighting ([32](#right-ref-B32)).

HT-DFT databases offer an attractive supplement to experimental databases for use in informatics as they can be resource efficient to build, comprehensive across chemistries, well structured, and internally consistent. For instance, identifying the DFT-calculable Debye temperature as a reliable indicator for the complex materials property of photoluminescent quantum yield enabled the use of an HT-DFT elastic tensor data set to predict novel light-emitting diode (LED) materials ([32](#right-ref-B32)). DFT, when coupled with active learning, can also be a rapid engine for exploring a design space and optimizing properties ([33](#right-ref-B33)).

2.2.  
Descriptor Representation

Any successful application of ML to materials discovery relies on a suitable choice of representation ([34](#right-ref-B34)). Representation refers to how a material is encoded in a machine-readable format, typically as a fixed-length vector of descriptors (also referred to as features or input variables). For instance, Ni3Al could be represented as simply the combination of character strings in the composition, the atomic coordinates of Ni and Al in the L12 crystal structure, or a scanning electron micrograph of the microstructure. Representation is an opportunity to inject known physical information into an ML prediction problem. For example, that Ni crystallizes in the face-centered cubic structure and has a melting point of 1,455°C can be directly exploited in differentiating Ni from other elements when training ML models. The choice of representation can have a large effect on ML model performance, as observed by Askerka et al. ([35](#right-ref-B35)) for the thermodynamic stability of double perovskites ([Figure 3](#f3)).

Figure 3 
Askerka et al. ([35](#right-ref-B35)) investigated the representation dependence of machine learning model predictions for double perovskite thermodynamic stability. Their learning-in-templates (LiT) approach assumes nominal atomic positions, which they compared to using optimized atomic positions. They benchmarked several crystal structure representations from the literature: radial distribution functions (RDF) and partial radial distribution functions (PRDF) ([36](#right-ref-B36)), density features and bond fractions ([37](#right-ref-B37)), the orbital field matrix ([38](#right-ref-B38)), and Voronoi tessellations ([39](#right-ref-B39)). Figure adapted with permission from Reference [35](#right-ref-B35). Copyright 2019, American Chemical Society.

[![
                     Figure 3 
                  ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/dfd50eac953bd89f7eb435a1d4cb169e.png)

Figure 3 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f3.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f3.ppt?mimeType=application/vnd.ms-powerpoint)

In the majority of case studies in [Table 1](#t1), researchers used simple empirical descriptors associated with the elemental compositions of materials under investigation. The magpie ([40](#right-ref-B40)) and matminer ([37](#right-ref-B37)) packages are widely used sources of these chemical features, which include physical concepts such as atomic size, electronegativity, and electron configuration. The selection of a high-quality representation is likely to be important for success in using ML for materials discovery.

Across many materials problems, the optimal choice of representation is nonobvious. For example, recent research ([41](#right-ref-B41), [42](#right-ref-B42)) has developed representations for the concept of a grain boundary, which may be intuitively clear to a human scientist but is not straightforwardly captured as a vector or matrix object suitable for linear algebra operations. Likewise, new atomic-scale representations for small molecules ([43](#right-ref-B43), [44](#right-ref-B44)), periodic systems (e.g., crystal structures) ([39](#right-ref-B39), [45](#right-ref-B45)), and combinations thereof ([34](#right-ref-B34), [46](#right-ref-B46)) are being actively developed.

Including as many descriptors as possible is one way to ensure that no known physics is left out of a modeling exercise. On the other hand, many ML algorithms are susceptible to degraded performance in the presence of correlated and/or meaningless descriptors ([47](#right-ref-B47)). The processes of dimensionality reduction [e.g., principal component analysis ([48](#right-ref-B48))] and feature selection aim to identify a reduced set of maximally informative and ideally uncorrelated descriptors for input to an ML model. For example, a metric called cluster resolution ([49](#right-ref-B49)), which uses the relative positions and geometries of clusters present in data sets to quantify the preservation of differences between various types of materials, was used to perform feature selection in several case studies listed in [Table 1](#t1).

2.3.  
Design Space and Cross-Validation

Cross-validation (CV), which quantifies the performance of ML models, can be customized to a desired design space in order to obtain realistic estimates of model performance for the discovery application at hand. The concept of design space refers to the chemistries, experimental conditions, and processing routes one is interested in searching for new materials. A critical question is the relationship between the training data and the design space; generally speaking, the more different these two regimes are, the more challenging ML-driven discovery will be.

2.3.1.  
Measuring model performance via cross-validation.

CV is the gold standard approach for quantifying the performance of ML models. In CV, models are trained on a subset of all available data and then used to predict values (for regression-type problems) or labels (for classification-type problems) for a held-out set of data for which the ground truth is known. Conceptually, CV is intended to probe an ML model's ability to generalize to unseen examples and embodies the idea that models should not be evaluated on data to which they were fit.

The most widely used form of CV is random k-fold, in which the available training data are randomly divided into k partitions (i.e., folds). Over k iterations, the ML model is trained on k − 1 partitions and used to predict the held-out partition. Performance metrics such as root mean square error (RMSE) or Pearson r
2 may be computed across all held-out partitions. Among the case studies in [Table 1](#t1), random k-fold CV is almost universally employed to compute these model accuracy statistics.

Interestingly, while random k-fold CV is widely used in both the ML research and materials informatics communities, materials discovery may pose challenges for traditional CV methods. In particular, because (a) materials data sets typically exhibit strong clustering and (b) materials discovery may involve extrapolation, random k-fold CV has a tendency to overestimate the performance of ML models ([50](#right-ref-B50)). CV techniques such as leave-one-cluster-out (LOCO) ([50](#right-ref-B50)) and leave-out-group (LOG) ([51](#right-ref-B51)) have emerged to simulate materials discovery use cases. Drug discovery researchers have made similar observations ([52](#right-ref-B52), [53](#right-ref-B53)), and appropriately matching CV techniques to the problem at hand remains an essential step in scientific applications of ML ([54](#right-ref-B54)).

2.3.2.  
Extrapolative design spaces.

Supervised ML approaches generally assume that all training data, along with unseen examples we wish to predict, are independent of one another and drawn from the same underlying distribution; this is the so-called independent and identically distributed (i.i.d.) assumption ([55](#right-ref-B55)). However, real-world materials discovery applications often strain the i.i.d. conditions. As mentioned in the preceding section, experiments may be clustered due to sampling bias. In particular, scientists tend to measure many small changes to a few successful parent materials and to heavily underreport failed materials. Further, we may be interested in designing materials with structures, chemistries, or properties very different from those reflected in our training data. We refer to these latter situations as extrapolation.

Based on this definition, extrapolative materials discovery may or may not actually violate the i.i.d. assumption. The key question is whether the physics associated with as-yet-undiscovered materials of interest is satisfactorily sampled in the training data. To take superconductors as an example, a training set of Bardeen–Cooper–Schrieffer materials does not at all sample the anomalous physics of the cuprates, and the i.i.d. assumption is catastrophically violated. Thus, as we would intuitively expect, an ML model trained on Bardeen–Cooper–Schrieffer superconductors has no predictive power whatsoever for the cuprates ([50](#right-ref-B50), [56](#right-ref-B56)). In this vein, none of the case studies in [Table 1](#t1) describe the discovery of entirely new physical regimes with ML, although ML-optimized sampling of chemical space can accelerate such discoveries beyond the pace of a purely random search ([57](#right-ref-B57)).

To illustrate an alternative scenario, imagine that we focus specifically on the discovery of materials with exceptional (i.e., extreme) values of certain properties. In this case, ML may be able to extrapolate beyond the property ranges present in the training data, if the necessary physics is present in the training data. However, this type of prediction problem is difficult. As shown in [Figure 4](#f4), an ML model for bulk modulus (B) based on the Materials Project elastic property database ([58](#right-ref-B58)) shows good performance over a range of B from 0 to 400 GPa when standard k-fold CV is applied. However, when an ML model is trained only with compounds with B < 300 GPa, the model's accuracy under extrapolation to greater values of B suffers.

Figure 4 
Example illustrating the effects of property extrapolation on ML model performance, using DFT-calculated mechanical property data from the Materials Project ([31](#right-ref-B31), [58](#right-ref-B58)). Blue circles show the results of typical CV across the entire data set, whereas orange triangles demonstrate the degradation in model performance that occurs when only materials with B < 300 GPa are used to train, and the remaining higher-B compounds are predicted. Abbreviations: CV, cross-validation; DFT, density functional theory; ML, machine learning.

[![
                        Figure 4 
                     ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/21f0a7bec2af339d7e6babb6bc3ca341.png)

Figure 4 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f4.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f4.ppt?mimeType=application/vnd.ms-powerpoint)

2.4.  
Machine Learning Algorithms

The choice of algorithm underlying trained models in materials informatics is one that is largely driven by the specific materials problem being addressed, i.e., the nature of the model inputs and the desired outputs. As seen in [Table 1](#t1), various algorithms have been successfully employed for various problems. The popular random forest (RF) ([59](#right-ref-B59), [60](#right-ref-B60)) and (deep) neural network (NN) ([61](#right-ref-B61), [62](#right-ref-B62)) algorithms are illustrated conceptually in [Figure 5](#f5).

Figure 5 
Schematic representation of (a) neural network and (b) random forest machine learning algorithms. In this hypothetical example, the models predict the band gap of an AB compound based on three features: the electronegativity difference between A and B (χA − χB), the atomic radius ratio between A and B (r
A/r
B), and the valence electron concentration (VEC) of the AB compound.

[![
                     Figure 5 
                  ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/b07e5cde1df57a23ae9c6f6d62ecc564.png)

Figure 5 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f5.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f5.ppt?mimeType=application/vnd.ms-powerpoint)

A NN consists of an interconnected set of logical gates, called neurons, to transform a series of input data into an output decision. NN models lend themselves to pattern matching when training data sets are substantial and complex. In the informatics use cases reviewed here, such training data sets consist of data generated from high-throughput physics-based simulations ([63](#right-ref-B63), [64](#right-ref-B64)). The series of logical decisions made by the NN enable reproduction of complex abrupt changes in output space given inputs, such as how a minor change in a simplified molecular-input line-entry system (SMILES) string can radically alter the rate constant ([64](#right-ref-B64)).

The RF algorithm trains multiple decision tree models on randomized bootstrapped subsets of the training data. Model predictions are then made based on the collected predictions of the decision trees. This results in a model robust to overfitting, which works well for the smaller data set sizes common in materials science, such as the ∼2,000 Heusler structures used to predict stability ([65](#right-ref-B65)) and the ∼6,800 compositions used to predict glass formability ([7](#right-ref-B7)). Two of the main advantages of the RF algorithm are robustness to sparse data and ease of performing feature selection.

Comparison of performance between these and other algorithms is a subject of study in the material informatics literature ([66](#right-ref-B66)) and is an important consideration when selecting one for a design problem. For instance, Gómez-Bombarelli et al. ([64](#right-ref-B64)) found that the NN algorithm dramatically outperformed linear regression for prediction of molecular organic light-emitting diode (OLED) performance when the training data set size grew large, which is expected for molecular design spaces. However, for continuous composition-dependent design spaces (such as inorganic solids) and smaller training data sets, algorithm choice becomes less significant for model performance. Iwasaki et al. ([67](#right-ref-B67)) and Wen et al. ([22](#right-ref-B22)) observed little change in RMSE between NN and RF models for inorganic solid property prediction. Xue et al. ([68](#right-ref-B68)) report similar prediction errors between various regression techniques, with polynomial regression being lower. However, in the context of discovery and design of experiments, RMSE and other simple error metrics are not necessarily the ideal performance criteria. Ultimately, trained models are a means to an end, and measuring the ability of a model to predict high-performance candidates is preferred. Gómez-Bombarelli et al. ([64](#right-ref-B64)), for instance, quantify this as the fraction of molecules in the test set correctly ranked in the top 5% of all molecules.

3.  CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

[Table 1](#t1) presents a selection of 23 applications of ML to materials discovery wherein the predictions from ML were subsequently confirmed by experiment or simulation. In the following subsections, we highlight some of the key aspects of these case studies that are likely to have contributed to verifiable success.

3.1.  
Augmenting Domain Expertise with Machine Learning

After his defeat by IBM's Deep Blue in 1997, chess champion Garry Kasparov concluded that great complementarity exists between human and computer intelligence. In 1998, Kasparov created advanced chess, a format in which humans play with the aid of a chess computer ([69](#right-ref-B69)). An analogous pairing of domain expertise and ML has led to several successes in materials design.

This concept of combining existing expert knowledge with ML to exploit complementarity can be powerful. While an unaided domain expert may simply miss an underlying trend in a large data set, ML can readily surface these patterns. Conversely, while an ML model is capable of generating massive numbers of candidate materials, a domain expert can sensibly prioritize materials for synthesis from the suggested list, taking into account, e.g., compatibility with laboratory equipment and economic factors that may be difficult to formally incorporate into ML models. Feedback from domain experts regarding predictive failures can also drive the subsequent refinement of ML models.

In an early example of the application of ML to materials discovery, Meredig et al. ([70](#right-ref-B70)) demonstrated that models trained on DFT calculations could very accurately predict the thermodynamic stability of new compounds. Interestingly, they found that a model that combined pure ML with a domain knowledge–derived heuristic outperformed either ML or the heuristic individually. The ML model used only chemical composition as input; the heuristic used information from binary phase diagrams to predict the stability of ternary phases. With ML and the heuristic together, Meredig et al. identified nine materials as candidates for discovery, and confirmed using DFT calculations that eight of these compounds were more energetically stable than any combinations of known materials ([70](#right-ref-B70)).

The work of Oliynyk et al. ([65](#right-ref-B65)) offers another instance of extending domain knowledge with ML. A common question that arises when ML is applied to materials discovery is whether the predictions from ML are “nonobvious,” and in this paper, Oliynyk et al. directly compare a pure electron-counting heuristic [akin to the 18-electron rule for half-Heuslers ([71](#right-ref-B71))] to the results of using electron counts plus many other descriptors in an ML model. Oliynyk et al. selected for synthesis several compounds whose likelihood of Heusler formation was predicted to be low by electron counting but high according to the ML model. The compounds TiRu2Ga, VRu2Ga, CrRu2Ga, RuTi2Ga, RuV2Ga, RuCr2Ga, and RuMn2Ga were experimentally confirmed to crystallize in the Heusler structure ([65](#right-ref-B65)), in spite of very low predicted probabilities from the electron count–only approach. [Figure 6](#f6) summarizes the discovery results of Oliynyk et al. This example illustrates how heuristics often used to identify “usual suspect” materials may miss interesting candidates that a more elaborate ML approach can successfully identify.

Figure 6 
Summary of the machine learning (ML)–driven discovery results of Oliynyk et al. ([65](#right-ref-B65)). Out of 14 ML-predicted high-probability Heusler compounds, 12 were experimentally confirmed; 7 predicted negatives were also verified in the laboratory. Adapted with permission from Reference [65](#right-ref-B65). Copyright 2016, American Chemical Society.

[![
                     Figure 6 
                  ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/14139e2bf5fd8363576651b8d27a5e2a.png)

Figure 6 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f6.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f6.ppt?mimeType=application/vnd.ms-powerpoint)

3.2.  
Combining Machine Learning with Physics-Based Simulations

Widely used physics-based simulations, such as DFT and molecular dynamics, are natural complements to ML for three primary reasons. First, as ML (especially in materials) is often starved for precious training data, physical simulations can generate realistic training examples in abundance. Second, ML algorithms have no innate knowledge of physics, and concurrent use of simulations can guard against unphysical or pathological behavior in ML models. Third, ML in the context of transfer learning (i.e., using an ML model trained on a larger data set to assist in a related prediction problem that has fewer training data available) can build predictive connections between simulation and laboratory experimentation ([72](#right-ref-B72)).

Work by Mansouri Tehrani et al. ([31](#right-ref-B31)) illustrates these points. In their effort to discover new earth-abundant superhard materials, these researchers trained ML models on approximately 2,500 DFT-calculated bulk (B) and shear (G) moduli ([73](#right-ref-B73)) in the Materials Project, generated consistently in a high-throughput fashion. Over 100,000 candidates were then screened for very large values of these elastic moduli. The training data were limited mainly to binary compounds due to the computational cost of DFT mechanical property calculations on more complex unit cells. Despite this restriction, the employed ML model successfully extrapolated into ternary and quaternary systems. Mansouri Tehrani et al.’s approach was informed by the fact that DFT mechanical property data are much more abundant than experimental data and by the observation that Vickers hardness (H
V) values tend to correlate with B and G ([74](#right-ref-B74)). This ML-driven screening process surfaced Mo0.9W1.1BC and Re0.5W0.5C as promising candidates, the highest predicted bulk modulus values of quaternary and ternary phases, respectively. Subsequent experiments confirmed that both materials exhibited superhard behavior (taken to be H
V > 40 GPa) at low load ([31](#right-ref-B31)).

Besides the DFT-based approach exemplified by Mansouri Tehrani et al. ([31](#right-ref-B31)), other physics-based or mechanistic models can be used as critical components in an informatics pipeline. Menon et al. ([75](#right-ref-B75)) utilize a suite of physicochemical models to transform an initially simple molecular candidate space, based on mixtures of only seven commercial polymers, into a complex space of physical parameters which determine how these mixtures plasticize cement. In this way, domain expertise and prior knowledge are encoded in these physical models, enabling a predictive model [in this case, least absolute shrinkage and selection operator (LASSO) ([76](#right-ref-B76))] from a more limited data set. Another example by Bucior et al. ([77](#right-ref-B77)) generates 3D H2 adsorption energy profiles for known metal–organic framework (MOF) structures using grand canonical Monte Carlo and Lennard-Jones plus Coulombic potentials. These 3D profiles were transformed into 1D histograms of adsorption energy, with the histogram bin heights used as the MOF descriptors for LASSO training. Interestingly, ignoring spatial dimensions of adsorption behavior did not diminish the model's ability to predict MOF performance.

3.3.  
Active Learning and Iterative Discovery

As is often the case in materials informatics problems, one starts with a limited quantity of training data on which to build a model in search of new materials in a large design space. Consequently, the initial model will likely be inadequate to describe the entirety of the design space. In such instances, iterative active learning approaches are useful to efficiently sample the design space for additional training data to collect. Active learning involves the use of a model's prediction uncertainties to identify the ideal candidate experiments to achieve a goal, either to broaden the model's applicability in the design space and improve accuracy (exploration) or to identify the highest-performing candidates (exploitation)—or some combination thereof. Upon execution of these suggested experiments, the resulting data are used to retrain and enhance the underlying ML model, such that the candidates in the next iteration are likelier to represent improvements. Active learning, when applied to materials data sets, has been shown to significantly reduce the number of experiments needed to identify the highest-performing material when compared to random guessing ([57](#right-ref-B57)).

Such an iterative approach was used by Ren et al. ([7](#right-ref-B7)) to efficiently develop a model for bulk metallic glass (BMG) formability in ternary metal systems and identify novel BMG-forming systems. The authors started with a training data set of 6,780 experimental reports, covering 293 ternary systems. The authors noted that most of these data come from only 38 ternary systems and are biased toward systems with known BMGs (i.e., a bias toward positive results). A classifier model for whether a ternary composition will form a BMG was trained on these data (first generation; [Figure 7](#f7)). The Co-V-Zr system was identified as a ternary with many novel BMG-forming compositions and experimentally validated by a combinatorial thin-film synthesis approach, which revealed a large glass region. These results were added to the training data, and the resulting model (second generation) has significantly superior performance to the first, as shown by the receiver operating characteristic curve in [Figure 7](#f7). Importantly, the authors attribute this fact to the considerable number of negative training data added, improving the data set quality for learning. Raccuglia et al. ([78](#right-ref-B78)) made a similar observation. For this reason, in the second round of model-selected experiments, a system predicted to not form BMGs (Fe-Ti-Nb) was synthesized alongside two that do (Co-Ti-Zr and Co-Fe-Zr), and the results agreed well with the second-generation model. Adding these new systems to the training data, a third-generation model exhibited further improvement over the second, particularly at low false-positive rate (i.e., true prediction of glass-forming systems).

Figure 7 
Receiver operating characteristic (ROC) curves illustrate a model's trade-off between true positives and false positives, where greater area under the ROC (AUROC) curve indicates superior performance. Ren et al. ([7](#right-ref-B7)) iteratively improved their machine learning (ML) models of bulk metallic glass (BMG) formability. The first-generation model contained only BMG data derived from the Landolt–Börnstein handbook ([79](#right-ref-B79)). The second and third generations introduced experimental data obtained in testing ML predictions. Adapted from Reference [7](#right-ref-B7). Copyright The Authors, some rights reserved; exclusive licensee American Association for the Advancement of Science. Distributed under a Creative Commons (CC BY-NC) license.

[![
                     Figure 7 
                  ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/e252eac0f6b134b4e2314bcba081205e.png)

Figure 7 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f7.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f7.ppt?mimeType=application/vnd.ms-powerpoint)

3.4.  
Identifying Materials Exhibiting Property Extrema

Because ML is often used in pattern-matching applications, it is particularly challenging to surface materials with property values that lie outside the range of any initially known training materials. However, in an example of successful property value extrapolation, Xue et al. ([68](#right-ref-B68)) found that a simple polynomial containing up to quadratic terms in three features (valence electron count, atomic radius, and electronegativity) could successfully extrapolate to much higher values of shape-memory alloy transition temperatures T
p than were present in the training data. The training data generated by the researchers contained T
p values no greater than approximately 100°C, but the model accurately predicted values extracted from the published literature that ranged up to nearly 300°C. Further, an experiment on a material whose predicted T
p was 189.56°C was found experimentally to have a transformation temperature of 182.89°C.

The case studies in [Table 1](#t1) contain several additional examples of using ML to design materials with property values outside the range of the initially available training data. In rare cases, these discoveries can be accomplished in a single shot, as was done by Xue et al. ([68](#right-ref-B68)). In many cases, an iterative active learning strategy must be employed. Rickman et al. ([17](#right-ref-B17)) and Wen et al. ([22](#right-ref-B22)) designed high-entropy alloys with measured hardness values greater than the alloys in their respective training sets. Sakurai et al. ([80](#right-ref-B80)) used Bayesian optimization to develop a layered metamaterial thermal radiator with a Q-factor higher than previously observed. Thus, with appropriate training data, and often also with the aid of active learning, ML can enable discovery of materials with extreme property values.

3.5.  
Designing for Multiple Properties

Materials discovery applications often do not involve optimizing only a single property of interest. Rather, real-world problems are inherently multiobjective, which is more complex than single-variable optimization. Most works take one of two approaches to this challenge: (a) passing materials candidates through a number of property screens, with the hope that a tractable list of candidates satisfies all of the screening criteria, or (b) applying scalarizing functions to transform a multiobjective design into a surrogate single-objective problem. The first approach assumes one can satisfactorily evaluate all properties for a preenumerated list of candidate materials; the second approach involves iteratively evaluating individual candidates or batches, and retraining ML models at each iteration.

The Li-ion battery electrolyte screening work of Sendek et al. ([81](#right-ref-B81)), which led to a case study ([82](#right-ref-B82)) in [Table 1](#t1), illustrates the screening strategy. Sendek et al. trained an ML model on experimental ionic conductivity values for Li-ion conductors and screened a DFT-derived database ([28](#right-ref-B28)) of candidate materials using this ML model along with a number of other criteria, as shown in [Figure 8](#f8). This multiproperty screening approach, which involved tabulated elemental properties, heuristics, and DFT calculations in addition to ML, reduced 12,831 candidate electrolytes to 12. Subsequent DFT calculations confirmed materials in the Li-B-S system to have extraordinarily high ionic conductivity values ([82](#right-ref-B82)).

Figure 8 
Multiproperty Li-ion battery electrolyte screening strategy of Sendek et al. ([81](#right-ref-B81)). A combination of physics-based simulation, economic and practicality arguments, and machine learning modeling reduced a list of 12,831 candidate materials to 12. Abbreviation: DFT, density functional theory. Figure adapted with permission from the Royal Society of Chemistry, from “Holistic computational structure screening of more than 12000 candidates for solid lithium-ion conductor materials,” Sendek et al., Energy Environ. Sci. 10(1) 2017 ([81](#right-ref-B81)); permission conveyed through Copyright Clearance Center, Inc.

[![
                     Figure 8 
                  ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/ac3862bffd54c87cf3c148665d33346c.png)

Figure 8 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f8.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f8.ppt?mimeType=application/vnd.ms-powerpoint)

Scalarizing functions are a second approach for multiproperty materials design, where multiple property requirements are combined into a single function. This strategy maps a multiobjective problem to a single-objective problem, which can then be solved with any standard optimization approach. For example, Häse et al. ([83](#right-ref-B83)) developed Chimera, which takes as user input a prioritized list of all materials properties under consideration (e.g., a user could specify that thermodynamic stability matters more than high ionic conductivity) and outputs a single-objective function suitable for optimization. In measuring the success of scalarizing functions, studies tend to focus on the Pareto optimality of surfaced candidates ([83](#right-ref-B83), [84](#right-ref-B84)). A candidate is Pareto optimal (or, equivalently, lies on the Pareto frontier) if there exists no other candidate that is superior across every property dimension. Thus, the candidates on the Pareto frontier each offer a unique set of trade-offs across properties of interest. For instance, two superconducting materials could be Pareto optimal if one offers a high critical temperature T
c but subpar ductility (important for making wires of the material), while the other possesses superior ductility but a lower T
c. As it is impossible, without user input, to declare a winner among Pareto-optimal materials, the ability to efficiently surface as many materials on the Pareto frontier as possible is a sensible benchmark for scalarizing functions.

3.6.  
Generating Novel Materials

For some materials development challenges, particularly those involving organic small-molecule design, the design space is so massive that it cannot be exhaustively enumerated. In such cases, if novel molecules are desired, the design space will be populated by either (a) candidates generated de novo via ML without any prior structural input, perhaps using variational autoencoders ([85](#right-ref-B85)), as illustrated in [Figure 9](#f9) ([86](#right-ref-B86)), or generative adversarial networks ([87](#right-ref-B87)); or (b) candidates generated from known constituent building blocks and filtered by rules or heuristics based on domain expertise. Of course, a third common route involves using a preexisting library of candidates, e.g., PubChem entries, but this strategy by definition will not yield any chemical novelty; it can only predict unknown properties of previously observed materials.

Figure 9 
Gómez-Bombarelli et al. ([86](#right-ref-B86)) utilized a variational autoencoder to encode molecular structures, as represented by SMILES strings, into a latent space that allows for continuous optimization of properties. A decoder then enables recovery of feasible molecules with human-interpretable SMILES representations. Abbreviation: SMILES, simplified molecular-input line-entry system. Adapted with permission from the American Chemical Society (ACS) from Reference [86](#right-ref-B86) (<https://pubs.acs.org/doi/10.1021/acscentsci.7b00572>); further permissions related to the material excerpted should be directed to the ACS.

[![
                     Figure 9 
                  ](ai-leaders-insights/产业应用与实践/科学发现/材料科学/images/de02f578e9f7e016006338061cb06dd0.png)

Figure 9 
  
  
Click to view](/docserver/fulltext/matsci/50/1/mr500049.f9.png)[Download as PowerPoint](/docserver/fulltext/matsci/50/1/mr500049.f9.ppt?mimeType=application/vnd.ms-powerpoint)

Chemical generation approaches were utilized in a pair of studies on OLED design. In the work of Gómez-Bombarelli et al. ([64](#right-ref-B64)), 222 moieties and several design rules based on electronic structure and synthesizability were used to generate 1.6 million candidate molecules. The SMILES representations for these molecules were converted into the fixed-length vector extended-connectivity fingerprint (ECFP) representation and used as input into a NN trained on k
TADF, a time-dependent DFT-derived OLED performance metric. The NN predicted k
TADF for all candidate molecules, the resulting list was ranked, and DFT was performed on the top-ranked candidates to validate the prediction and add to the training data. After each iteration, the improved NN was used to identify top candidates, which were further downselected for experiment.

Kim et al. ([63](#right-ref-B63)) dynamically generated candidate OLED structures through a pair of NNs. For their inverse design pipeline, they trained a deep NN on the DFT-predicted electronic properties of 50,000 randomly selected structures from the PubChem database. This deep NN then predicted the electronic properties of randomly generated ECFP vectors. For the top-performing candidates, a recurrent NN converted the ECFP vector into a SMILES string. If the SMILES string corresponded to a chemically valid structure, Kim et al. ran DFT on the structure, and recommended those structures exceeding performance targets for subsequent experimental investigation. The authors ran this pipeline until they had identified 1,500 molecules satisfying their design constraints. Approximately 10% existed in PubChem but were not present in the training set, suggesting that the pipeline is capable of reproducing molecules found by traditional chemistry expertise.

4.  CONCLUSION

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

ML is beginning to exert a major impact on materials discovery. In [Table 1](#f1), we highlighted a number of ML discovery case studies across a wide variety of materials applications. In areas ranging from small molecules to metal alloys, ML predictions have subsequently been confirmed by laboratory experiment or, in some cases, validated via physics-based simulations. In this review, we identified some strategies that have lent themselves to success in ML-aided materials discovery, such as explicitly combining domain knowledge with ML modeling. We also discussed the underlying components of a typical materials informatics discovery pipeline, such as high-quality input data and carefully selected materials representations.

Looking ahead, we anticipate important work in several areas of materials informatics. First, we must confront the issue of profound data scarcity in materials science; here, autonomous materials research ([88](#right-ref-B88)), wherein ML-driven robotic synthesis and characterization apparatuses run in closed-loop fashion, could play a major role. Autonomy is particularly interesting because the time required for experimentation (i.e., data generation) is a severe bottleneck in the materials development process. Second, ML model interpretability, which enables researchers to gain greater physical insight from using ML models, will broaden the appeal and applicability of ML as a scientific tool. ML models are often considered black boxes ([89](#right-ref-B89)) because the process by which inputs are transformed into outputs is opaque for many ML algorithms, but greater interpretability would ameliorate this limitation. Finally, we should be able to quantify the behavior of ML models during extrapolative materials discovery. In particular, design space optimization could maximize the likelihood that ML will find nonobvious, high-performing materials. If we can optimize where we are searching for discoveries, accelerate our rate of data generation, and enhance the transparency of ML models for scientific users, ML will be transformative for our ability to discover and design groundbreaking new materials.

disclosure statement

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

The authors are not aware of any affiliations, memberships, funding, or financial holdings that might be perceived as affecting the objectivity of this review.

literature cited

Go to section...

* [TOP](#top-1)
* [ABSTRACT](#abstract-1)
* [INTRODUCTION](#sec1)
* [THE MATERIALS INFORMATICS DISCOVERY PIPELINE](#sec2)
* [CONFIRMED PREDICTIONS WITH METHODOLOGICAL HIGHLIGHTS](#sec3)
* [CONCLUSION](#sec4)
* [disclosure statement](#sec5)
* [literature cited](#sec6)

1. 1.

   Hill J, Mulholland G, Persson K, Seshadri R, Wolverton C, Meredig B 2016.  Materials science with large-scale data and informatics: unlocking new opportunities.  MRS Bull 41:399–409

   [[Crossref]](https://doi.org/10.1557/mrs.2016.93)
   [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000375926200013&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+science+with+large-scale+data+and+informatics%3A+unlocking+new+opportunities&author=J+Hill&author=G+Mulholland&author=K+Persson&author=R+Seshadri&author=C+Wolverton&author=B+Meredig&journal=MRS+Bull&volume=41&doi=10.1557%2Fmrs.2016.93&pages=399-409&publication_year=2016&)
2. 2.

   Jain A, Hautier G, Ong SP, Persson K 2016.  New opportunities for materials informatics: resources and data mining techniques for uncovering hidden relationships.  J. Mater. Res. 31:977–94

   [[Crossref]](https://doi.org/10.1557/jmr.2016.80)
   [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000376178000001&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=New+opportunities+for+materials+informatics%3A+resources+and+data+mining+techniques+for+uncovering+hidden+relationships&author=A+Jain&author=G+Hautier&author=SP+Ong&author=K+Persson&journal=J.+Mater.+Res.&volume=31&doi=10.1557%2Fjmr.2016.80&pages=977-94&publication_year=2016&)
3. 3.

   Mueller T, Kusne AG, Ramprasad R 2016.  Machine learning in materials science: recent progress and emerging applications.  Rev. Comput. Chem. 29:186–273


   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+in+materials+science%3A+recent+progress+and+emerging+applications&author=T+Mueller&author=AG+Kusne&author=R+Ramprasad&journal=Rev.+Comput.+Chem.&volume=29&pages=186-273&publication_year=2016&)
4. 4.

   Ramprasad R, Batra R, Pilania G, Mannodi-Kanakkithodi A, Kim C 2017.  Machine learning in materials informatics: recent applications and prospects.  npj Comput. Mater. 3:54

   [[Crossref]](https://doi.org/10.1038/s41524-017-0056-5)
   [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426838500001&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+in+materials+informatics%3A+recent+applications+and+prospects&author=R+Ramprasad&author=R+Batra&author=G+Pilania&author=A+Mannodi-Kanakkithodi&author=C+Kim&journal=npj+Comput.+Mater.&volume=3&doi=10.1038%2Fs41524-017-0056-5&pages=54&publication_year=2017&)
5. 5.

   Butler KT, Davies DW, Cartwright H, Isayev O, Walsh A 2018.  Machine learning for molecular and materials science.  Nature 559:547–55

   [[Crossref]](https://doi.org/10.1038/s41586-018-0337-2)

   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+for+molecular+and+materials+science&author=KT+Butler&author=DW+Davies&author=H+Cartwright&author=O+Isayev&author=A+Walsh&journal=Nature&volume=559&doi=10.1038%2Fs41586-018-0337-2&pages=547-55&publication_year=2018&)
6. 6.

   Larsen P, Von Ins M 2010.  The rate of growth in scientific publication and the decline in coverage provided by science citation index.  Scientometrics 84:575–603

   [[Crossref]](https://doi.org/10.1007/s11192-010-0202-z)
   [[Medline]](https://pubmed.ncbi.nlm.nih.gov/20700371) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000280274400003&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=The+rate+of+growth+in+scientific+publication+and+the+decline+in+coverage+provided+by+science+citation+index&author=P+Larsen&author=M+Von+Ins&journal=Scientometrics&volume=84&doi=10.1007%2Fs11192-010-0202-z&pages=575-603&publication_year=2010&)
7. 7.

   Ren F, Ward L, Williams T, Laws KJ, Wolverton C et al. 2018.  Accelerated discovery of metallic glasses through iteration of machine learning and high-throughput experiments.  Sci. Adv. 4:eaaq1566

   [[Crossref]](https://doi.org/10.1126/sciadv.aaq1566)
   [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29662953) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000431374900043&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Accelerated+discovery+of+metallic+glasses+through+iteration+of+machine+learning+and+high-throughput+experiments&author=F+Ren&author=L+Ward&author=T+Williams&author=KJ+Laws&author=C+Wolverton&journal=Sci.+Adv.&volume=4&doi=10.1126%2Fsciadv.aaq1566&pages=eaaq1566&publication_year=2018&)
8. 8.

   Abadi M, Agarwal A, Barham P, Brevdo E, Chen Z et al. 2016.  TensorFlow: large-scale machine learning on heterogeneous distributed systems.  arXiv:1603.04467 [cs]
9. 9.

   Allen FH. 2002.  The Cambridge Structural Database: a quarter of a million crystal structures and rising.  Acta Crystallogr. B 58:380–88

   [[Crossref]](https://doi.org/10.1107/S0108768102003890)
   [[Medline]](https://pubmed.ncbi.nlm.nih.gov/12037359) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000176270700010&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=The+Cambridge+Structural+Database%3A+a+quarter+of+a+million+crystal+structures+and+rising&author=FH.+Allen&journal=Acta+Crystallogr.+B&volume=58&doi=10.1107%2FS0108768102003890&pages=380-88&publication_year=2002&)
10. 10.

    Seiler KP, George GA, Happ MP, Bodycombe NE, Carrinski HA et al. 2007.  ChemBank: a small-molecule screening and cheminformatics resource database.  Nucleic Acids Res 36:D351–59

    [[Crossref]](https://doi.org/10.1093/nar/gkm843)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/17947324) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000252545400064&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=ChemBank%3A+a+small-molecule+screening+and+cheminformatics+resource+database&author=KP+Seiler&author=GA+George&author=MP+Happ&author=NE+Bodycombe&author=HA+Carrinski&journal=Nucleic+Acids+Res&volume=36&doi=10.1093%2Fnar%2Fgkm843&pages=D351-59&publication_year=2007&)
11. 11.

    Benson DA, Karsch-Mizrachi I, Lipman DJ, Ostell J, Sayers EW 2008.  GenBank.  Nucleic Acids Res 37:D26–31

    [[Crossref]](https://doi.org/10.1093/nar/gkn723)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000261906200005&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=GenBank&author=DA+Benson&author=I+Karsch-Mizrachi&author=DJ+Lipman&author=J+Ostell&author=EW+Sayers&journal=Nucleic+Acids+Res&volume=37&doi=10.1093%2Fnar%2Fgkn723&pages=D26-31&publication_year=2008&)
12. 12.

    Kim S, Thiessen PA, Bolton EE, Chen J, Fu G et al. 2015.  PubChem substance and compound databases.  Nucleic Acids Res 44:D1202–13

    [[Crossref]](https://doi.org/10.1093/nar/gkv951)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26400175) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000371261700170&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=PubChem+substance+and+compound+databases&author=S+Kim&author=PA+Thiessen&author=EE+Bolton&author=J+Chen&author=G+Fu&journal=Nucleic+Acids+Res&volume=44&doi=10.1093%2Fnar%2Fgkv951&pages=D1202-13&publication_year=2015&)
13. 13.

    Blaiszik B, Chard K, Pruyne J, Ananthakrishnan R, Tuecke S, Foster I 2016.  The materials data facility: data services to advance materials science research.  JOM 68:2045–52

    [[Crossref]](https://doi.org/10.1007/s11837-016-2001-3)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000381991400010&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=The+materials+data+facility%3A+data+services+to+advance+materials+science+research&author=B+Blaiszik&author=K+Chard&author=J+Pruyne&author=R+Ananthakrishnan&author=S+Tuecke&author=I+Foster&journal=JOM&volume=68&doi=10.1007%2Fs11837-016-2001-3&pages=2045-52&publication_year=2016&)
14. 14.

    Draxl C, Scheffler M. 2018.  NOMAD: the FAIR concept for big data–driven materials science.  MRS Bull 43:676–82

    [[Crossref]](https://doi.org/10.1557/mrs.2018.208)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=NOMAD%3A+the+FAIR+concept+for+big+data%E2%80%93driven+materials+science&author=C+Draxl&author=M.+Scheffler&journal=MRS+Bull&volume=43&doi=10.1557%2Fmrs.2018.208&pages=676-82&publication_year=2018&)
15. 15.

    O'Mara J, Meredig B, Michel K 2016.  Materials data infrastructure: a case study of the Citrination platform to examine data import, storage, and access.  JOM 68:2031–34

    [[Crossref]](https://doi.org/10.1007/s11837-016-1984-0)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000381991400008&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+data+infrastructure%3A+a+case+study+of+the+Citrination+platform+to+examine+data+import%2C+storage%2C+and+access&author=J+O%27Mara&author=B+Meredig&author=K+Michel&journal=JOM&volume=68&doi=10.1007%2Fs11837-016-1984-0&pages=2031-34&publication_year=2016&)
16. 16.

    Seshadri R, Sparks TD. 2016.  Perspective: interactive material property databases through aggregation of literature data.  APL Mater 4:053206

    [[Crossref]](https://doi.org/10.1063/1.4944682)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000377720400010&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Perspective%3A+interactive+material+property+databases+through+aggregation+of+literature+data&author=R+Seshadri&author=TD.+Sparks&journal=APL+Mater&volume=4&doi=10.1063%2F1.4944682&pages=053206&publication_year=2016&)
17. 17.

    Rickman J, Chan H, Harmer M, Smeltzer J, Marvel C et al. 2019.  Materials informatics for the screening of multi-principal elements and high-entropy alloys.  Nat. Commun. 10:2618

    [[Crossref]](https://doi.org/10.1038/s41467-019-10533-1)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+informatics+for+the+screening+of+multi-principal+elements+and+high-entropy+alloys&author=J+Rickman&author=H+Chan&author=M+Harmer&author=J+Smeltzer&author=C+Marvel&journal=Nat.+Commun.&volume=10&doi=10.1038%2Fs41467-019-10533-1&pages=2618&publication_year=2019&)
18. 18.

    Iwasaki Y, Takeuchi I, Stanev V, Kusne AG, Ishida M et al. 2019.  Machine-learning guided discovery of a new thermoelectric material.  Sci. Rep. 9:2751

    [[Crossref]](https://doi.org/10.1038/s41598-019-39278-z)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine-learning+guided+discovery+of+a+new+thermoelectric+material&author=Y+Iwasaki&author=I+Takeuchi&author=V+Stanev&author=AG+Kusne&author=M+Ishida&journal=Sci.+Rep.&volume=9&doi=10.1038%2Fs41598-019-39278-z&pages=2751&publication_year=2019&)
19. 19.

    Balachandran PV, Kowalski B, Sehirlioglu A, Lookman T 2018.  Experimental search for high-temperature ferroelectric perovskites guided by two-step machine learning.  Nat. Commun. 9:1668

    [[Crossref]](https://doi.org/10.1038/s41467-018-03821-9)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29700297) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000430922400001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Experimental+search+for+high-temperature+ferroelectric+perovskites+guided+by+two-step+machine+learning&author=PV+Balachandran&author=B+Kowalski&author=A+Sehirlioglu&author=T+Lookman&journal=Nat.+Commun.&volume=9&doi=10.1038%2Fs41467-018-03821-9&pages=1668&publication_year=2018&)
20. 20.

    Min K, Choi B, Park K, Cho E 2018.  Machine learning assisted optimization of electrochemical properties for Ni-rich cathode materials.  Sci. Rep. 8:15778

    [[Crossref]](https://doi.org/10.1038/s41598-018-34201-4)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+assisted+optimization+of+electrochemical+properties+for+Ni-rich+cathode+materials&author=K+Min&author=B+Choi&author=K+Park&author=E+Cho&journal=Sci.+Rep.&volume=8&doi=10.1038%2Fs41598-018-34201-4&pages=15778&publication_year=2018&)
21. 21.

    Hatakeyama-Sato K, Tezuka T, Nishikitani Y, Nishide H, Oyaizu K 2018.  Synthesis of lithium-ion conducting polymers designed by machine learning–based prediction and screening.  Chem. Lett. 48:130–32

    [[Crossref]](https://doi.org/10.1246/cl.180847)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Synthesis+of+lithium-ion+conducting+polymers+designed+by+machine+learning%E2%80%93based+prediction+and+screening&author=K+Hatakeyama-Sato&author=T+Tezuka&author=Y+Nishikitani&author=H+Nishide&author=K+Oyaizu&journal=Chem.+Lett.&volume=48&doi=10.1246%2Fcl.180847&pages=130-32&publication_year=2018&)
22. 22.

    Wen C, Zhang Y, Wang C, Xue D, Bai Y et al. 2019.  Machine learning assisted design of high entropy alloys with desired property.  Acta Mater 170:109–17

    [[Crossref]](https://doi.org/10.1016/j.actamat.2019.03.010)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+assisted+design+of+high+entropy+alloys+with+desired+property&author=C+Wen&author=Y+Zhang&author=C+Wang&author=D+Xue&author=Y+Bai&journal=Acta+Mater&volume=170&doi=10.1016%2Fj.actamat.2019.03.010&pages=109-17&publication_year=2019&)
23. 23.

    Hohenberg P, Kohn W. 1964.  Inhomogeneous electron gas.  Phys. Rev. B 136:864–71

    [[Crossref]](https://doi.org/10.1103/PhysRev.136.B864)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Inhomogeneous+electron+gas&author=P+Hohenberg&author=W.+Kohn&journal=Phys.+Rev.+B&volume=136&doi=10.1103%2FPhysRev.136.B864&pages=864-71&publication_year=1964&)
24. 24.

    Kohn W, Sham LJ. 1965.  Self-consistent equations including exchange and correlation effects.  Phys. Rev. A 140:1133–38

    [[Crossref]](https://doi.org/10.1103/PhysRev.140.A1133)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Self-consistent+equations+including+exchange+and+correlation+effects&author=W+Kohn&author=LJ.+Sham&journal=Phys.+Rev.+A&volume=140&doi=10.1103%2FPhysRev.140.A1133&pages=1133-38&publication_year=1965&)
25. 25.

    Kresse G, Hafner J. 1993.  Ab initio molecular dynamics for liquid metals.  Phys. Rev. B 47:558–61

    [[Crossref]](https://doi.org/10.1103/PhysRevB.47.558)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Ab+initio+molecular+dynamics+for+liquid+metals&author=G+Kresse&author=J.+Hafner&journal=Phys.+Rev.+B&volume=47&doi=10.1103%2FPhysRevB.47.558&pages=558-61&publication_year=1993&)
26. 26.

    Hafner J. 2008.  Ab-initio simulations of materials using VASP: density-functional theory and beyond.  J. Comput. Chem. 29:2044–78

    [[Crossref]](https://doi.org/10.1002/jcc.21057)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/18623101) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000258764600002&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Ab-initio+simulations+of+materials+using+VASP%3A+density-functional+theory+and+beyond&author=J.+Hafner&journal=J.+Comput.+Chem.&volume=29&doi=10.1002%2Fjcc.21057&pages=2044-78&publication_year=2008&)
27. 27.

    Curtarolo S, Setyawan W, Wang S, Xue J, Yang K et al. 2012.  Aflowlib.org: a distributed materials properties repository from high-throughput ab initio calculations.  Comput. Mater. Sci. 58:227–35

    [[Crossref]](https://doi.org/10.1016/j.commatsci.2012.02.002)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000302118400031&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Aflowlib.org%3A+a+distributed+materials+properties+repository+from+high-throughput+ab+initio+calculations&author=S+Curtarolo&author=W+Setyawan&author=S+Wang&author=J+Xue&author=K+Yang&journal=Comput.+Mater.+Sci.&volume=58&doi=10.1016%2Fj.commatsci.2012.02.002&pages=227-35&publication_year=2012&)
28. 28.

    Jain A, Ong SP, Hautier G, Chen W, Richards WD et al. 2013.  Commentary: The materials project: a materials genome approach to accelerating materials innovation.  APL Mater 1:011002

    [[Crossref]](https://doi.org/10.1063/1.4812323)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000332272300003&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Commentary%3A+The+materials+project%3A+a+materials+genome+approach+to+accelerating+materials+innovation&author=A+Jain&author=SP+Ong&author=G+Hautier&author=W+Chen&author=WD+Richards&journal=APL+Mater&volume=1&doi=10.1063%2F1.4812323&pages=011002&publication_year=2013&)
29. 29.

    Saal JE, Kirklin S, Aykol M, Meredig B, Wolverton C 2013.  Materials design and discovery with high-throughput density functional theory: the Open Quantum Materials Database (OQMD).  JOM 65:1501–9

    [[Crossref]](https://doi.org/10.1007/s11837-013-0755-4)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000327496400020&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+design+and+discovery+with+high-throughput+density+functional+theory%3A+the+Open+Quantum+Materials+Database+%28OQMD%29&author=JE+Saal&author=S+Kirklin&author=M+Aykol&author=B+Meredig&author=C+Wolverton&journal=JOM&volume=65&doi=10.1007%2Fs11837-013-0755-4&pages=1501-9&publication_year=2013&)
30. 30.

    Ward L, Aykol M, Blaiszik B, Foster I, Meredig B et al. 2018.  Strategies for accelerating the adoption of materials informatics.  MRS Bull 43:683–89

    [[Crossref]](https://doi.org/10.1557/mrs.2018.204)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Strategies+for+accelerating+the+adoption+of+materials+informatics&author=L+Ward&author=M+Aykol&author=B+Blaiszik&author=I+Foster&author=B+Meredig&journal=MRS+Bull&volume=43&doi=10.1557%2Fmrs.2018.204&pages=683-89&publication_year=2018&)
31. 31.

    Mansouri Tehrani A, Oliynyk AO, Parry M, Rizvi Z, Couper S et al. 2018.  Machine learning directed search for ultraincompressible, superhard materials.  J. Am. Chem. Soc. 140:9844–53

    [[Crossref]](https://doi.org/10.1021/jacs.8b02717)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+directed+search+for+ultraincompressible%2C+superhard+materials&author=A+Mansouri+Tehrani&author=AO+Oliynyk&author=M+Parry&author=Z+Rizvi&author=S+Couper&journal=J.+Am.+Chem.+Soc.&volume=140&doi=10.1021%2Fjacs.8b02717&pages=9844-53&publication_year=2018&)
32. 32.

    Zhuo Y, Mansouri Tehrani A, Oliynyk AO, Duke AC, Brgoch J 2018.  Identifying an efficient, thermally robust inorganic phosphor host via machine learning.  Nat. Commun. 9:4377

    [[Crossref]](https://doi.org/10.1038/s41467-018-06625-z)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Identifying+an+efficient%2C+thermally+robust+inorganic+phosphor+host+via+machine+learning&author=Y+Zhuo&author=A+Mansouri+Tehrani&author=AO+Oliynyk&author=AC+Duke&author=J+Brgoch&journal=Nat.+Commun.&volume=9&doi=10.1038%2Fs41467-018-06625-z&pages=4377&publication_year=2018&)
33. 33.

    Bassman L, Rajak P, Kalia RK, Nakano A, Sha F et al. 2018.  Active learning for accelerated design of layered materials.  npj Comput. Mater. 4:74

    [[Crossref]](https://doi.org/10.1038/s41524-018-0129-0)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Active+learning+for+accelerated+design+of+layered+materials&author=L+Bassman&author=P+Rajak&author=RK+Kalia&author=A+Nakano&author=F+Sha&journal=npj+Comput.+Mater.&volume=4&doi=10.1038%2Fs41524-018-0129-0&pages=74&publication_year=2018&)
34. 34.

    Huo H, Rupp M. 2017.  Unified representation for machine learning of molecules and crystals.  arXiv:1704.06439 [physics.chem-ph]
35. 35.

    Askerka M, Li Z, Lempen M, Liu Y, Johnston A et al. 2019.  Learning-in-templates enables accelerated discovery and synthesis of new stable double perovskites.  J. Am. Chem. Soc. 141:3682–90

    [[Crossref]](https://doi.org/10.1021/jacs.8b13420)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Learning-in-templates+enables+accelerated+discovery+and+synthesis+of+new+stable+double+perovskites&author=M+Askerka&author=Z+Li&author=M+Lempen&author=Y+Liu&author=A+Johnston&journal=J.+Am.+Chem.+Soc.&volume=141&doi=10.1021%2Fjacs.8b13420&pages=3682-90&publication_year=2019&)
36. 36.

    Schütt K, Glawe H, Brockherde F, Sanna A, Müller K, Gross E 2014.  How to represent crystal structures for machine learning: towards fast prediction of electronic properties.  Phys. Rev. B 89:205118

    [[Crossref]](https://doi.org/10.1103/PhysRevB.89.205118)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000336248300003&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=How+to+represent+crystal+structures+for+machine+learning%3A+towards+fast+prediction+of+electronic+properties&author=K+Sch%C3%BCtt&author=H+Glawe&author=F+Brockherde&author=A+Sanna&author=K+M%C3%BCller&author=E+Gross&journal=Phys.+Rev.+B&volume=89&doi=10.1103%2FPhysRevB.89.205118&pages=205118&publication_year=2014&)
37. 37.

    Ward L, Dunn A, Faghaninia A, Zimmermann NE, Bajaj S et al. 2018.  Matminer: an open source toolkit for materials data mining.  Comput. Mater. Sci. 152:60–69

    [[Crossref]](https://doi.org/10.1016/j.commatsci.2018.05.018)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Matminer%3A+an+open+source+toolkit+for+materials+data+mining&author=L+Ward&author=A+Dunn&author=A+Faghaninia&author=NE+Zimmermann&author=S+Bajaj&journal=Comput.+Mater.+Sci.&volume=152&doi=10.1016%2Fj.commatsci.2018.05.018&pages=60-69&publication_year=2018&)
38. 38.

    Faber FA, Christensen AS, Huang B, von Lilienfeld OA 2018.  Alchemical and structural distribution based representation for universal quantum machine learning.  J. Chem. Phys. 148:241717

    [[Crossref]](https://doi.org/10.1063/1.5020710)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29960351) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000437190300020&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Alchemical+and+structural+distribution+based+representation+for+universal+quantum+machine+learning&author=FA+Faber&author=AS+Christensen&author=B+Huang&author=OA+von+Lilienfeld&journal=J.+Chem.+Phys.&volume=148&doi=10.1063%2F1.5020710&pages=241717&publication_year=2018&)
39. 39.

    Ward L, Liu R, Krishna A, Hegde VI, Agrawal A et al. 2017.  Including crystal structure attributes in machine learning models of formation energies via Voronoi tessellations.  Phys. Rev. B 96:024104

    [[Crossref]](https://doi.org/10.1103/PhysRevB.96.024104)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000405509100001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Including+crystal+structure+attributes+in+machine+learning+models+of+formation+energies+via+Voronoi+tessellations&author=L+Ward&author=R+Liu&author=A+Krishna&author=VI+Hegde&author=A+Agrawal&journal=Phys.+Rev.+B&volume=96&doi=10.1103%2FPhysRevB.96.024104&pages=024104&publication_year=2017&)
40. 40.

    Ward L, Agrawal A, Choudhary A, Wolverton C 2016.  A general-purpose machine learning framework for predicting properties of inorganic materials.  npj Comput. Mater. 2:16028

    [[Crossref]](https://doi.org/10.1038/npjcompumats.2016.28)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426821500024&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=A+general-purpose+machine+learning+framework+for+predicting+properties+of+inorganic+materials&author=L+Ward&author=A+Agrawal&author=A+Choudhary&author=C+Wolverton&journal=npj+Comput.+Mater.&volume=2&doi=10.1038%2Fnpjcompumats.2016.28&pages=16028&publication_year=2016&)
41. 41.

    Rosenbrock CW, Homer ER, Csányi G, Hart GL 2017.  Discovering the building blocks of atomic systems using machine learning: application to grain boundaries.  npj Comput. Mater. 3:29

    [[Crossref]](https://doi.org/10.1038/s41524-017-0027-x)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426833500001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Discovering+the+building+blocks+of+atomic+systems+using+machine+learning%3A+application+to+grain+boundaries&author=CW+Rosenbrock&author=ER+Homer&author=G+Cs%C3%A1nyi&author=GL+Hart&journal=npj+Comput.+Mater.&volume=3&doi=10.1038%2Fs41524-017-0027-x&pages=29&publication_year=2017&)
42. 42.

    Gomberg JA, Medford AJ, Kalidindi SR 2017.  Extracting knowledge from molecular mechanics simulations of grain boundaries using machine learning.  Acta Mater 133:100–8

    [[Crossref]](https://doi.org/10.1016/j.actamat.2017.05.009)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000407413100011&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Extracting+knowledge+from+molecular+mechanics+simulations+of+grain+boundaries+using+machine+learning&author=JA+Gomberg&author=AJ+Medford&author=SR+Kalidindi&journal=Acta+Mater&volume=133&doi=10.1016%2Fj.actamat.2017.05.009&pages=100-8&publication_year=2017&)
43. 43.

    Gilmer J, Schoenholz SS, Riley PF, Vinyals O, Dahl GE 2017.  Neural message passing for quantum chemistry.  Proceedings of the 34th International Conference on Machine Learning D Precup, YW Teh 1263–72 New York: ACM <https://dl.acm.org/doi/10.5555/3305381.3305512>


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Neural+message+passing+for+quantum+chemistry&author=J+Gilmer&author=SS+Schoenholz&author=PF+Riley&author=O+Vinyals&author=GE+Dahl&journal=Proceedings+of+the+34th+International+Conference+on+Machine+Learning&pages=1263-72&publication_year=2017&)
44. 44.

    Schütt KT, Sauceda HE, Kindermans PJ, Tkatchenko A, Müller KR 2018.  SchNet—a deep learning architecture for molecules and materials.  J. Chem. Phys. 148:241722

    [[Crossref]](https://doi.org/10.1063/1.5019779)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29960322) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000437190300025&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=SchNet%E2%80%94a+deep+learning+architecture+for+molecules+and+materials&author=KT+Sch%C3%BCtt&author=HE+Sauceda&author=PJ+Kindermans&author=A+Tkatchenko&author=KR+M%C3%BCller&journal=J.+Chem.+Phys.&volume=148&doi=10.1063%2F1.5019779&pages=241722&publication_year=2018&)
45. 45.

    Xie T, Grossman JC. 2018.  Crystal graph convolutional neural networks for an accurate and interpretable prediction of material properties.  Phys. Rev. Lett. 120:145301

    [[Crossref]](https://doi.org/10.1103/PhysRevLett.120.145301)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29694125) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000429451000012&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Crystal+graph+convolutional+neural+networks+for+an+accurate+and+interpretable+prediction+of+material+properties&author=T+Xie&author=JC.+Grossman&journal=Phys.+Rev.+Lett.&volume=120&doi=10.1103%2FPhysRevLett.120.145301&pages=145301&publication_year=2018&)
46. 46.

    Bartók AP, De S, Poelking C, Bernstein N, Kermode JR et al. 2017.  Machine learning unifies the modeling of materials and molecules.  Sci. Adv. 3:e1701816

    [[Crossref]](https://doi.org/10.1126/sciadv.1701816)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29242828) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000418003100020&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+unifies+the+modeling+of+materials+and+molecules&author=AP+Bart%C3%B3k&author=S+De&author=C+Poelking&author=N+Bernstein&author=JR+Kermode&journal=Sci.+Adv.&volume=3&doi=10.1126%2Fsciadv.1701816&pages=e1701816&publication_year=2017&)
47. 47.

    Hall MA. 1999. Correlation-based feature selection for machine learning PhD Thesis, Univ. Waikato Hamilton, N. Z:.


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Correlation-based+feature+selection+for+machine+learning&author=MA.+Hall&publication_year=1999&)
48. 48.

    Jolliffe IT, Cadima J. 2016.  Principal component analysis: a review and recent developments.  Philos. Trans. R. Soc. A 374:20150202

    [[Crossref]](https://doi.org/10.1098/rsta.2015.0202)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26953178) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000372553500008&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Principal+component+analysis%3A+a+review+and+recent+developments&author=IT+Jolliffe&author=J.+Cadima&journal=Philos.+Trans.+R.+Soc.+A&volume=374&doi=10.1098%2Frsta.2015.0202&pages=20150202&publication_year=2016&)
49. 49.

    Sinkov NA, Harynuk JJ. 2011.  Cluster resolution: a metric for automated, objective and optimized feature selection in chemometric modeling.  Talanta 83:1079–87

    [[Crossref]](https://doi.org/10.1016/j.talanta.2010.10.025)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/21215842) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000286718700004&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Cluster+resolution%3A+a+metric+for+automated%2C+objective+and+optimized+feature+selection+in+chemometric+modeling&author=NA+Sinkov&author=JJ.+Harynuk&journal=Talanta&volume=83&doi=10.1016%2Fj.talanta.2010.10.025&pages=1079-87&publication_year=2011&)
50. 50.

    Meredig B, Antono E, Church C, Hutchinson M, Ling J et al. 2018.  Can machine learning identify the next high-temperature superconductor? Examining extrapolation performance for materials discovery.  Mol. Syst. Des. Eng. 3:819–25

    [[Crossref]](https://doi.org/10.1039/C8ME00012C)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Can+machine+learning+identify+the+next+high-temperature+superconductor%3F+Examining+extrapolation+performance+for+materials+discovery&author=B+Meredig&author=E+Antono&author=C+Church&author=M+Hutchinson&author=J+Ling&journal=Mol.+Syst.+Des.+Eng.&volume=3&doi=10.1039%2FC8ME00012C&pages=819-25&publication_year=2018&)
51. 51.

    Lu HJ, Zou N, Jacobs R, Afflerbach B, Lu XG, Morgan D 2019.  Error assessment and optimal cross-validation approaches in machine learning applied to impurity diffusion.  Comput. Mater. Sci. 169:109075

    [[Crossref]](https://doi.org/10.1016/j.commatsci.2019.06.010)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Error+assessment+and+optimal+cross-validation+approaches+in+machine+learning+applied+to+impurity+diffusion&author=HJ+Lu&author=N+Zou&author=R+Jacobs&author=B+Afflerbach&author=XG+Lu&author=D+Morgan&journal=Comput.+Mater.+Sci.&volume=169&doi=10.1016%2Fj.commatsci.2019.06.010&pages=109075&publication_year=2019&)
52. 52.

    Sheridan RP. 2013.  Time-split cross-validation as a method for estimating the goodness of prospective prediction.  J. Chem. Inf. Model. 53:783–90

    [[Crossref]](https://doi.org/10.1021/ci400084k)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/23521722) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000318060200006&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Time-split+cross-validation+as+a+method+for+estimating+the+goodness+of+prospective+prediction&author=RP.+Sheridan&journal=J.+Chem.+Inf.+Model.&volume=53&doi=10.1021%2Fci400084k&pages=783-90&publication_year=2013&)
53. 53.

    Wallach I, Heifets A. 2018.  Most ligand-based classification benchmarks reward memorization rather than generalization.  J. Chem. Inf. Model. 58:916–32

    [[Crossref]](https://doi.org/10.1021/acs.jcim.7b00403)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29698607) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000433634900004&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Most+ligand-based+classification+benchmarks+reward+memorization+rather+than+generalization&author=I+Wallach&author=A.+Heifets&journal=J.+Chem.+Inf.+Model.&volume=58&doi=10.1021%2Facs.jcim.7b00403&pages=916-32&publication_year=2018&)
54. 54.

    Riley P. 2019.  Three pitfalls to avoid in machine learning.  Nature 572:27–29

    [[Crossref]](https://doi.org/10.1038/d41586-019-02307-y)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Three+pitfalls+to+avoid+in+machine+learning&author=P.+Riley&journal=Nature&volume=572&doi=10.1038%2Fd41586-019-02307-y&pages=27-29&publication_year=2019&)
55. 55.

    Vapnik VN. 1999.  An overview of statistical learning theory.  IEEE Trans. Neural Netw. 10:988–99

    [[Crossref]](https://doi.org/10.1109/72.788640)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=An+overview+of+statistical+learning+theory&author=VN.+Vapnik&journal=IEEE+Trans.+Neural+Netw.&volume=10&doi=10.1109%2F72.788640&pages=988-99&publication_year=1999&)
56. 56.

    Stanev V, Oses C, Kusne AG, Rodriguez E, Paglione J et al. 2018.  Machine learning modeling of superconducting critical temperature.  npj Comput. Mater. 4:29

    [[Crossref]](https://doi.org/10.1038/s41524-018-0085-8)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000438373200001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+modeling+of+superconducting+critical+temperature&author=V+Stanev&author=C+Oses&author=AG+Kusne&author=E+Rodriguez&author=J+Paglione&journal=npj+Comput.+Mater.&volume=4&doi=10.1038%2Fs41524-018-0085-8&pages=29&publication_year=2018&)
57. 57.

    Ling J, Hutchinson M, Antono E, Paradiso S, Meredig B 2017.  High-dimensional materials and process optimization using data-driven experimental design with well-calibrated uncertainty estimates.  Integr. Mater. Manuf. Innov. 6:207–17

    [[Crossref]](https://doi.org/10.1007/s40192-017-0098-z)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000411716600001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=High-dimensional+materials+and+process+optimization+using+data-driven+experimental+design+with+well-calibrated+uncertainty+estimates&author=J+Ling&author=M+Hutchinson&author=E+Antono&author=S+Paradiso&author=B+Meredig&journal=Integr.+Mater.+Manuf.+Innov.&volume=6&doi=10.1007%2Fs40192-017-0098-z&pages=207-17&publication_year=2017&)
58. 58.

    De Jong M, Chen W, Angsten T, Jain A, Notestine R et al. 2015.  Charting the complete elastic properties of inorganic crystalline compounds.  Sci. Data 2:150009

    [[Crossref]](https://doi.org/10.1038/sdata.2015.9)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/25984348) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000390328900001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Charting+the+complete+elastic+properties+of+inorganic+crystalline+compounds&author=M+De+Jong&author=W+Chen&author=T+Angsten&author=A+Jain&author=R+Notestine&journal=Sci.+Data&volume=2&doi=10.1038%2Fsdata.2015.9&pages=150009&publication_year=2015&)
59. 59.

    Breiman L. 2001.  Random forests.  Mach. Learn. 45:5–32

    [[Crossref]](https://doi.org/10.1023/A:1010933404324)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Random+forests&author=L.+Breiman&journal=Mach.+Learn.&volume=45&doi=10.1023%2FA%3A1010933404324&pages=5-32&publication_year=2001&)
60. 60.

    Wager S, Hastie T, Efron B 2014.  Confidence intervals for random forests: the jackknife and the infinitesimal jackknife.  J. Mach. Learn. Res. 15:1625–51


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Confidence+intervals+for+random+forests%3A+the+jackknife+and+the+infinitesimal+jackknife&author=S+Wager&author=T+Hastie&author=B+Efron&journal=J.+Mach.+Learn.+Res.&volume=15&pages=1625-51&publication_year=2014&)
61. 61.

    Krogh A, Vedelsby J. 1996.  Neural network ensembles, cross validation, and active learning.  Advances in Neural Information Processing Systems 8 (NIPS 1995) DS Touretzky, MC Mozer, ME Hasselmo 231–38 Cambridge, MA: MIT Press


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Neural+network+ensembles%2C+cross+validation%2C+and+active+learning&author=A+Krogh&author=J.+Vedelsby&journal=Advances+in+Neural+Information+Processing+Systems+8+%28NIPS+1995%29&pages=231-38&publication_year=1996&)
62. 62.

    LeCun Y, Bengio Y, Hinton G 2015.  Deep learning.  Nature 521:436–44

    [[Crossref]](https://doi.org/10.1038/nature14539)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26017442) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000355286600030&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Deep+learning&author=Y+LeCun&author=Y+Bengio&author=G+Hinton&journal=Nature&volume=521&doi=10.1038%2Fnature14539&pages=436-44&publication_year=2015&)
63. 63.

    Kim K, Kang S, Yoo J, Kwon Y, Nam Y et al. 2018.  Deep-learning-based inverse design model for intelligent discovery of organic molecules.  npj Comput. Mater. 4:67

    [[Crossref]](https://doi.org/10.1038/s41524-018-0128-1)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Deep-learning-based+inverse+design+model+for+intelligent+discovery+of+organic+molecules&author=K+Kim&author=S+Kang&author=J+Yoo&author=Y+Kwon&author=Y+Nam&journal=npj+Comput.+Mater.&volume=4&doi=10.1038%2Fs41524-018-0128-1&pages=67&publication_year=2018&)
64. 64.

    Gómez-Bombarelli R, Aguilera-Iparraguirre J, Hirzel TD, Duvenaud D, Maclaurin D et al. 2016.  Design of efficient molecular organic light-emitting diodes by a high-throughput virtual screening and experimental approach.  Nat. Mater. 15:1120–27

    [[Crossref]](https://doi.org/10.1038/nmat4717)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Design+of+efficient+molecular+organic+light-emitting+diodes+by+a+high-throughput+virtual+screening+and+experimental+approach&author=R+G%C3%B3mez-Bombarelli&author=J+Aguilera-Iparraguirre&author=TD+Hirzel&author=D+Duvenaud&author=D+Maclaurin&journal=Nat.+Mater.&volume=15&doi=10.1038%2Fnmat4717&pages=1120-27&publication_year=2016&)
65. 65.

    Oliynyk AO, Antono E, Sparks TD, Ghadbeigi L, Gaultois MW et al. 2016.  High-throughput machine-learning-driven synthesis of full-Heusler compounds.  Chem. Mater. 28:7324–31

    [[Crossref]](https://doi.org/10.1021/acs.chemmater.6b02724)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000386421900018&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=High-throughput+machine-learning-driven+synthesis+of+full-Heusler+compounds&author=AO+Oliynyk&author=E+Antono&author=TD+Sparks&author=L+Ghadbeigi&author=MW+Gaultois&journal=Chem.+Mater.&volume=28&doi=10.1021%2Facs.chemmater.6b02724&pages=7324-31&publication_year=2016&)
66. 66.

    Agrawal A, Deshpande PD, Cecen A, Basavarsu GP, Choudhary AN, Kalidindi SR 2014.  Exploration of data science techniques to predict fatigue strength of steel from composition and processing parameters.  Integr. Mater. Manuf. Innov. 3:90–108

    [[Crossref]](https://doi.org/10.1186/2193-9772-3-8)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Exploration+of+data+science+techniques+to+predict+fatigue+strength+of+steel+from+composition+and+processing+parameters&author=A+Agrawal&author=PD+Deshpande&author=A+Cecen&author=GP+Basavarsu&author=AN+Choudhary&author=SR+Kalidindi&journal=Integr.+Mater.+Manuf.+Innov.&volume=3&doi=10.1186%2F2193-9772-3-8&pages=90-108&publication_year=2014&)
67. 67.

    Iwasaki Y, Sawada R, Stanev V, Ishida M, Kirihara A et al. 2019.  Materials development by interpretable machine learning.  arXiv:1903.02175 [cond-mat.mtrl-sci]
68. 68.

    Xue D, Xue D, Yuan R, Zhou Y, Balachandran PV et al. 2017.  An informatics approach to transformation temperatures of NiTi-based shape memory alloys.  Acta Mater 125:532–41

    [[Crossref]](https://doi.org/10.1016/j.actamat.2016.12.009)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000394201500054&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=An+informatics+approach+to+transformation+temperatures+of+NiTi-based+shape+memory+alloys&author=D+Xue&author=D+Xue&author=R+Yuan&author=Y+Zhou&author=PV+Balachandran&journal=Acta+Mater&volume=125&doi=10.1016%2Fj.actamat.2016.12.009&pages=532-41&publication_year=2017&)
69. 69.

    Hassabis D. 2017.  Artificial intelligence: chess match of the century.  Nature 544:413–14

    [[Crossref]](https://doi.org/10.1038/544413a)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000400051900019&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Artificial+intelligence%3A+chess+match+of+the+century&author=D.+Hassabis&journal=Nature&volume=544&doi=10.1038%2F544413a&pages=413-14&publication_year=2017&)
70. 70.

    Meredig B, Agrawal A, Kirklin S, Saal JE, Doak J et al. 2014.  Combinatorial screening for new materials in unconstrained composition space with machine learning.  Phys. Rev. B 89:094104

    [[Crossref]](https://doi.org/10.1103/PhysRevB.89.094104)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000332759000001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Combinatorial+screening+for+new+materials+in+unconstrained+composition+space+with+machine+learning&author=B+Meredig&author=A+Agrawal&author=S+Kirklin&author=JE+Saal&author=J+Doak&journal=Phys.+Rev.+B&volume=89&doi=10.1103%2FPhysRevB.89.094104&pages=094104&publication_year=2014&)
71. 71.

    Zeier WG, Anand S, Huang L, He R, Zhang H et al. 2017.  Using the 18-electron rule to understand the nominal 19-electron half-Heusler NbCoSb with Nb vacancies.  Chem. Mater. 29:1210–17

    [[Crossref]](https://doi.org/10.1021/acs.chemmater.6b04583)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000394924100039&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Using+the+18-electron+rule+to+understand+the+nominal+19-electron+half-Heusler+NbCoSb+with+Nb+vacancies&author=WG+Zeier&author=S+Anand&author=L+Huang&author=R+He&author=H+Zhang&journal=Chem.+Mater.&volume=29&doi=10.1021%2Facs.chemmater.6b04583&pages=1210-17&publication_year=2017&)
72. 72.

    Hutchinson ML, Antono E, Gibbons BM, Paradiso S, Ling J, Meredig B 2017.  Overcoming data scarcity with transfer learning.  arXiv:1711.05099 [cs.LG]
73. 73.

    De S, Bartók AP, Csányi G, Ceriotti M 2016.  Comparing molecules and solids across structural and alchemical space.  Phys. Chem. Chem. Phys. 18:13754–69

    [[Crossref]](https://doi.org/10.1039/C6CP00415F)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Comparing+molecules+and+solids+across+structural+and+alchemical+space&author=S+De&author=AP+Bart%C3%B3k&author=G+Cs%C3%A1nyi&author=M+Ceriotti&journal=Phys.+Chem.+Chem.+Phys.&volume=18&doi=10.1039%2FC6CP00415F&pages=13754-69&publication_year=2016&)
74. 74.

    Liu AY, Cohen ML. 1989.  Prediction of new low compressibility solids.  Science 245:841–42

    [[Crossref]](https://doi.org/10.1126/science.245.4920.841)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Prediction+of+new+low+compressibility+solids&author=AY+Liu&author=ML.+Cohen&journal=Science&volume=245&doi=10.1126%2Fscience.245.4920.841&pages=841-42&publication_year=1989&)
75. 75.

    Menon A, Childs CM, Poczós B, Washburn NR, Kurtis KE 2019.  Molecular engineering of superplasticizers for metakaolin-portland cement blends with hierarchical machine learning.  Adv. Theory Simul. 2:1800164

    [[Crossref]](https://doi.org/10.1002/adts.201800164)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Molecular+engineering+of+superplasticizers+for+metakaolin-portland+cement+blends+with+hierarchical+machine+learning&author=A+Menon&author=CM+Childs&author=B+Pocz%C3%B3s&author=NR+Washburn&author=KE+Kurtis&journal=Adv.+Theory+Simul.&volume=2&doi=10.1002%2Fadts.201800164&pages=1800164&publication_year=2019&)
76. 76.

    Santosa F, Symes WW. 1986.  Linear inversion of band-limited reflection seismograms.  SIAM J. Sci. Stat. Comput. 7:1307–30

    [[Crossref]](https://doi.org/10.1137/0907087)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Linear+inversion+of+band-limited+reflection+seismograms&author=F+Santosa&author=WW.+Symes&journal=SIAM+J.+Sci.+Stat.+Comput.&volume=7&doi=10.1137%2F0907087&pages=1307-30&publication_year=1986&)
77. 77.

    Bucior BJ, Bobbitt NS, Islamoglu T, Goswami S, Gopalan A et al. 2019.  Energy-based descriptors to rapidly predict hydrogen storage in metal–organic frameworks.  Mol. Syst. Des. Eng. 4:162–74

    [[Crossref]](https://doi.org/10.1039/C8ME00050F)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Energy-based+descriptors+to+rapidly+predict+hydrogen+storage+in+metal%E2%80%93organic+frameworks&author=BJ+Bucior&author=NS+Bobbitt&author=T+Islamoglu&author=S+Goswami&author=A+Gopalan&journal=Mol.+Syst.+Des.+Eng.&volume=4&doi=10.1039%2FC8ME00050F&pages=162-74&publication_year=2019&)
78. 78.

    Raccuglia P, Elbert KC, Adler PD, Falk C, Wenny MB et al. 2016.  Machine-learning-assisted materials discovery using failed experiments.  Nature 533:73–76

    [[Crossref]](https://doi.org/10.1038/nature17439)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/27147027) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000375473900041&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine-learning-assisted+materials+discovery+using+failed+experiments&author=P+Raccuglia&author=KC+Elbert&author=PD+Adler&author=C+Falk&author=MB+Wenny&journal=Nature&volume=533&doi=10.1038%2Fnature17439&pages=73-76&publication_year=2016&)
79. 79.

    Kawazoe Y, Yu J-Z, Tsai A-P, Masumoto T 1997. Phase Diagrams and Physical Properties of Nonequilibrium Alloys, Subvol. A: Nonequilibrium Phase Diagrams of Ternary Amorphous Alloys Landolt–Börnstein Numer. Data Funct. Relatsh. Sci. Technol. 37 Berlin/Heidelberg/New York: Springer


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Phase+Diagrams+and+Physical+Properties+of+Nonequilibrium+Alloys%2C+Subvol.+A%3A+Nonequilibrium+Phase+Diagrams+of+Ternary+Amorphous+Alloys&author=Y+Kawazoe&author=J-Z+Yu&author=A-P+Tsai&author=T+Masumoto&publication_year=1997&)
80. 80.

    Sakurai A, Yada K, Simomura T, Ju S, Kashiwagi M et al. 2019.  Ultranarrow-band wavelength-selective thermal emission with aperiodic multilayered metamaterials designed by Bayesian optimization.  ACS Cent. Sci. 5:319–26

    [[Crossref]](https://doi.org/10.1021/acscentsci.8b00802)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Ultranarrow-band+wavelength-selective+thermal+emission+with+aperiodic+multilayered+metamaterials+designed+by+Bayesian+optimization&author=A+Sakurai&author=K+Yada&author=T+Simomura&author=S+Ju&author=M+Kashiwagi&journal=ACS+Cent.+Sci.&volume=5&doi=10.1021%2Facscentsci.8b00802&pages=319-26&publication_year=2019&)
81. 81.

    Sendek AD, Yang Q, Cubuk ED, Duerloo KAN, Cui Y, Reed EJ 2017.  Holistic computational structure screening of more than 12,000 candidates for solid lithium-ion conductor materials.  Energy Environ. Sci. 10:306–20

    [[Crossref]](https://doi.org/10.1039/C6EE02697D)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Holistic+computational+structure+screening+of+more+than+12%2C000+candidates+for+solid+lithium-ion+conductor+materials&author=AD+Sendek&author=Q+Yang&author=ED+Cubuk&author=KAN+Duerloo&author=Y+Cui&author=EJ+Reed&journal=Energy+Environ.+Sci.&volume=10&doi=10.1039%2FC6EE02697D&pages=306-20&publication_year=2017&)
82. 82.

    Sendek AD, Antoniuk ER, Cubuk ED, Francisco BE, Buettner-Garrett J et al. 2019.  A new solid Li-ion electrolyte from the crystalline lithium-boron-sulfur system.  SSRN Electron. J. <https://dx.doi.org/10.2139/ssrn.3404263>

    [[Crossref]](https://doi.org/10.2139/ssrn.3404263)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=A+new+solid+Li-ion+electrolyte+from+the+crystalline+lithium-boron-sulfur+system&author=AD+Sendek&author=ER+Antoniuk&author=ED+Cubuk&author=BE+Francisco&author=J+Buettner-Garrett&journal=SSRN+Electron.+J.&doi=10.2139%2Fssrn.3404263&publication_year=2019&)
83. 83.

    Häse F, Roch LM, Aspuru-Guzik A 2018.  Chimera: enabling hierarchy based multi-objective optimization for self-driving laboratories.  Chem. Sci. 9:7642–55

    [[Crossref]](https://doi.org/10.1039/C8SC02239A)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Chimera%3A+enabling+hierarchy+based+multi-objective+optimization+for+self-driving+laboratories&author=F+H%C3%A4se&author=LM+Roch&author=A+Aspuru-Guzik&journal=Chem.+Sci.&volume=9&doi=10.1039%2FC8SC02239A&pages=7642-55&publication_year=2018&)
84. 84.

    Solomou A, Zhao G, Boluki S, Joy JK, Qian X et al. 2018.  Multi-objective Bayesian materials discovery: application on the discovery of precipitation strengthened NiTi shape memory alloys through micromechanical modeling.  Mater. Des. 160:810–27

    [[Crossref]](https://doi.org/10.1016/j.matdes.2018.10.014)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Multi-objective+Bayesian+materials+discovery%3A+application+on+the+discovery+of+precipitation+strengthened+NiTi+shape+memory+alloys+through+micromechanical+modeling&author=A+Solomou&author=G+Zhao&author=S+Boluki&author=JK+Joy&author=X+Qian&journal=Mater.+Des.&volume=160&doi=10.1016%2Fj.matdes.2018.10.014&pages=810-27&publication_year=2018&)
85. 85.

    Kingma DP, Welling M. 2013.  Auto-encoding variational Bayes.  arXiv:1312.6114 [stat.ML]
86. 86.

    Gómez-Bombarelli R, Wei JN, Duvenaud D, Hernández-Lobato JM, Sánchez-Lengeling B et al. 2018.  Automatic chemical design using a data-driven continuous representation of molecules.  ACS Cent. Sci. 4:268–76

    [[Crossref]](https://doi.org/10.1021/acscentsci.7b00572)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29532027) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426613700019&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Automatic+chemical+design+using+a+data-driven+continuous+representation+of+molecules&author=R+G%C3%B3mez-Bombarelli&author=JN+Wei&author=D+Duvenaud&author=JM+Hern%C3%A1ndez-Lobato&author=B+S%C3%A1nchez-Lengeling&journal=ACS+Cent.+Sci.&volume=4&doi=10.1021%2Facscentsci.7b00572&pages=268-76&publication_year=2018&)
87. 87.

    Goodfellow I, Pouget-Abadie J, Mirza M, Xu B, Warde-Farley D et al. 2014.  Generative adversarial nets.  Advances in Neural Information Processing Systems 27 (NIPS 2014) Z Ghahramani, M Welling, C Cortes, ND Lawrence, KQ Weinberger San Diego: Neural Inf. Process. Syst.


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Generative+adversarial+nets&author=I+Goodfellow&author=J+Pouget-Abadie&author=M+Mirza&author=B+Xu&author=D+Warde-Farley&journal=Advances+in+Neural+Information+Processing+Systems+27+%28NIPS+2014%29&publication_year=2014&)
88. 88.

    Nikolaev P, Hooper D, Webber F, Rao R, Decker K et al. 2016.  Autonomy in materials research: a case study in carbon nanotube growth.  npj Comput. Mater. 2:16031

    [[Crossref]](https://doi.org/10.1038/npjcompumats.2016.31)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426821500026&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Autonomy+in+materials+research%3A+a+case+study+in+carbon+nanotube+growth&author=P+Nikolaev&author=D+Hooper&author=F+Webber&author=R+Rao&author=K+Decker&journal=npj+Comput.+Mater.&volume=2&doi=10.1038%2Fnpjcompumats.2016.31&pages=16031&publication_year=2016&)
89. 89.

    Holm EA. 2019.  In defense of the black box.  Science 364:26–27

    [[Crossref]](https://doi.org/10.1126/science.aax0162)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=In+defense+of+the+black+box&author=EA.+Holm&journal=Science&volume=364&doi=10.1126%2Fscience.aax0162&pages=26-27&publication_year=2019&)
90. 90.

    Mannodi-Kanakkithodi A, Pilania G, Huan TD, Lookman T, Ramprasad R 2016.  Machine learning strategy for accelerated design of polymer dielectrics.  Sci. Rep. 6:20952

    [[Crossref]](https://doi.org/10.1038/srep20952)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26876223) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000370055400001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+strategy+for+accelerated+design+of+polymer+dielectrics&author=A+Mannodi-Kanakkithodi&author=G+Pilania&author=TD+Huan&author=T+Lookman&author=R+Ramprasad&journal=Sci.+Rep.&volume=6&doi=10.1038%2Fsrep20952&pages=20952&publication_year=2016&)
91. 91.

    Oliynyk AO, Adutwum LA, Harynuk JJ, Mar A 2016.  Classifying crystal structures of binary compounds AB through cluster resolution feature selection and support vector machine analysis.  Chem. Mater. 28:6672–81

    [[Crossref]](https://doi.org/10.1021/acs.chemmater.6b02905)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000384399000033&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Classifying+crystal+structures+of+binary+compounds+AB+through+cluster+resolution+feature+selection+and+support+vector+machine+analysis&author=AO+Oliynyk&author=LA+Adutwum&author=JJ+Harynuk&author=A+Mar&journal=Chem.+Mater.&volume=28&doi=10.1021%2Facs.chemmater.6b02905&pages=6672-81&publication_year=2016&)
92. 92.

    Villars P 2007. Pearson's Crystal Data®: crystal structure database for inorganic compounds. Database, ASM Int Materials Park, OH:


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Pearson%27s+Crystal+Data%C2%AE%3A+crystal+structure+database+for+inorganic+compounds.&author=P+Villars&publication_year=2007&)
93. 93.

    Oliynyk AO, Adutwum LA, Rudyk BW, Pisavadia H, Lotfi S et al. 2017.  Disentangling structural confusion through machine learning: structure prediction and polymorphism of equiatomic ternary phases ABC.  J. Am. Chem. Soc. 139:17870–81

    [[Crossref]](https://doi.org/10.1021/jacs.7b08460)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29129069) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000418204600033&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Disentangling+structural+confusion+through+machine+learning%3A+structure+prediction+and+polymorphism+of+equiatomic+ternary+phases+ABC&author=AO+Oliynyk&author=LA+Adutwum&author=BW+Rudyk&author=H+Pisavadia&author=S+Lotfi&journal=J.+Am.+Chem.+Soc.&volume=139&doi=10.1021%2Fjacs.7b08460&pages=17870-81&publication_year=2017&)
94. 94.

    Seko A, Hayashi H, Kashima H, Tanaka I 2018.  Matrix-and tensor-based recommender systems for the discovery of currently unknown inorganic compounds.  Phys. Rev. Mater. 2:013805

    [[Crossref]](https://doi.org/10.1103/PhysRevMaterials.2.013805)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000423135500002&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Matrix-and+tensor-based+recommender+systems+for+the+discovery+of+currently+unknown+inorganic+compounds&author=A+Seko&author=H+Hayashi&author=H+Kashima&author=I+Tanaka&journal=Phys.+Rev.+Mater.&volume=2&doi=10.1103%2FPhysRevMaterials.2.013805&pages=013805&publication_year=2018&)
95. 95.

    Belsky A, Hellenbrandt M, Karen VL, Luksch P 2002.  New developments in the Inorganic Crystal Structure Database (ICSD): accessibility in support of materials research and design.  Acta Crystallogr. B 58:364–69

    [[Crossref]](https://doi.org/10.1107/S0108768102006948)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/12037357) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000176270700008&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=New+developments+in+the+Inorganic+Crystal+Structure+Database+%28ICSD%29%3A+accessibility+in+support+of+materials+research+and+design&author=A+Belsky&author=M+Hellenbrandt&author=VL+Karen&author=P+Luksch&journal=Acta+Crystallogr.+B&volume=58&doi=10.1107%2FS0108768102006948&pages=364-69&publication_year=2002&)
96. 96.

    Lu S, Zhou Q, Ouyang Y, Guo Y, Li Q, Wang J 2018.  Accelerated discovery of stable lead-free hybrid organic–inorganic perovskites via machine learning.  Nat. Commun. 9:3405

    [[Crossref]](https://doi.org/10.1038/s41467-018-05761-w)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Accelerated+discovery+of+stable+lead-free+hybrid+organic%E2%80%93inorganic+perovskites+via+machine+learning&author=S+Lu&author=Q+Zhou&author=Y+Ouyang&author=Y+Guo&author=Q+Li&author=J+Wang&journal=Nat.+Commun.&volume=9&doi=10.1038%2Fs41467-018-05761-w&pages=3405&publication_year=2018&)
97. 97.

    Wu S, Kondo Y, Kakimoto M, Yang B, Yamada H et al. 2019.  Machine-learning-assisted discovery of polymers with high thermal conductivity using a molecular design algorithm.  npj Comput. Mater. 5:66

    [[Crossref]](https://doi.org/10.1038/s41524-019-0203-2)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine-learning-assisted+discovery+of+polymers+with+high+thermal+conductivity+using+a+molecular+design+algorithm&author=S+Wu&author=Y+Kondo&author=M+Kakimoto&author=B+Yang&author=H+Yamada&journal=npj+Comput.+Mater.&volume=5&doi=10.1038%2Fs41524-019-0203-2&pages=66&publication_year=2019&)
98. 98.

    Otsuka S, Kuwajima I, Hosoya J, Xu Y, Yamazaki M 2011.  PoLyInfo: polymer database for polymeric materials design.  2011 International Conference on Emerging Intelligent Data and Web Technologies22–29 Piscataway, NJ: IEEE


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=PoLyInfo%3A+polymer+database+for+polymeric+materials+design&author=S+Otsuka&author=I+Kuwajima&author=J+Hosoya&author=Y+Xu&author=M+Yamazaki&journal=2011+International+Conference+on+Emerging+Intelligent+Data+and+Web+Technologies&pages=22-29&publication_year=2011&)
99. 99.

    Ramakrishnan R, Dral PO, Rupp M, Von Lilienfeld OA 2014.  Quantum chemistry structures and properties of 134 kilo molecules.  Sci. Data 1:140022

    [[Crossref]](https://doi.org/10.1038/sdata.2014.22)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/25977779) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000209843500015&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Quantum+chemistry+structures+and+properties+of+134+kilo+molecules&author=R+Ramakrishnan&author=PO+Dral&author=M+Rupp&author=OA+Von+Lilienfeld&journal=Sci.+Data&volume=1&doi=10.1038%2Fsdata.2014.22&pages=140022&publication_year=2014&)

Copyright © 2020 by Annual Reviews. All rights reserved

[[Citing articles]](#)

[[Web of Science]](#)

[[Medline]](#)

Literature Cited

1. 1.

   Hill J, Mulholland G, Persson K, Seshadri R, Wolverton C, Meredig B 2016.  Materials science with large-scale data and informatics: unlocking new opportunities.  MRS Bull 41:399–409

   [[Crossref]](https://doi.org/10.1557/mrs.2016.93)
   [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000375926200013&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+science+with+large-scale+data+and+informatics%3A+unlocking+new+opportunities&author=J+Hill&author=G+Mulholland&author=K+Persson&author=R+Seshadri&author=C+Wolverton&author=B+Meredig&journal=MRS+Bull&volume=41&doi=10.1557%2Fmrs.2016.93&pages=399-409&publication_year=2016&)
2. 2.

   Jain A, Hautier G, Ong SP, Persson K 2016.  New opportunities for materials informatics: resources and data mining techniques for uncovering hidden relationships.  J. Mater. Res. 31:977–94

   [[Crossref]](https://doi.org/10.1557/jmr.2016.80)
   [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000376178000001&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=New+opportunities+for+materials+informatics%3A+resources+and+data+mining+techniques+for+uncovering+hidden+relationships&author=A+Jain&author=G+Hautier&author=SP+Ong&author=K+Persson&journal=J.+Mater.+Res.&volume=31&doi=10.1557%2Fjmr.2016.80&pages=977-94&publication_year=2016&)
3. 3.

   Mueller T, Kusne AG, Ramprasad R 2016.  Machine learning in materials science: recent progress and emerging applications.  Rev. Comput. Chem. 29:186–273


   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+in+materials+science%3A+recent+progress+and+emerging+applications&author=T+Mueller&author=AG+Kusne&author=R+Ramprasad&journal=Rev.+Comput.+Chem.&volume=29&pages=186-273&publication_year=2016&)
4. 4.

   Ramprasad R, Batra R, Pilania G, Mannodi-Kanakkithodi A, Kim C 2017.  Machine learning in materials informatics: recent applications and prospects.  npj Comput. Mater. 3:54

   [[Crossref]](https://doi.org/10.1038/s41524-017-0056-5)
   [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426838500001&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+in+materials+informatics%3A+recent+applications+and+prospects&author=R+Ramprasad&author=R+Batra&author=G+Pilania&author=A+Mannodi-Kanakkithodi&author=C+Kim&journal=npj+Comput.+Mater.&volume=3&doi=10.1038%2Fs41524-017-0056-5&pages=54&publication_year=2017&)
5. 5.

   Butler KT, Davies DW, Cartwright H, Isayev O, Walsh A 2018.  Machine learning for molecular and materials science.  Nature 559:547–55

   [[Crossref]](https://doi.org/10.1038/s41586-018-0337-2)

   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+for+molecular+and+materials+science&author=KT+Butler&author=DW+Davies&author=H+Cartwright&author=O+Isayev&author=A+Walsh&journal=Nature&volume=559&doi=10.1038%2Fs41586-018-0337-2&pages=547-55&publication_year=2018&)
6. 6.

   Larsen P, Von Ins M 2010.  The rate of growth in scientific publication and the decline in coverage provided by science citation index.  Scientometrics 84:575–603

   [[Crossref]](https://doi.org/10.1007/s11192-010-0202-z)
   [[Medline]](https://pubmed.ncbi.nlm.nih.gov/20700371) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000280274400003&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=The+rate+of+growth+in+scientific+publication+and+the+decline+in+coverage+provided+by+science+citation+index&author=P+Larsen&author=M+Von+Ins&journal=Scientometrics&volume=84&doi=10.1007%2Fs11192-010-0202-z&pages=575-603&publication_year=2010&)
7. 7.

   Ren F, Ward L, Williams T, Laws KJ, Wolverton C et al. 2018.  Accelerated discovery of metallic glasses through iteration of machine learning and high-throughput experiments.  Sci. Adv. 4:eaaq1566

   [[Crossref]](https://doi.org/10.1126/sciadv.aaq1566)
   [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29662953) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000431374900043&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Accelerated+discovery+of+metallic+glasses+through+iteration+of+machine+learning+and+high-throughput+experiments&author=F+Ren&author=L+Ward&author=T+Williams&author=KJ+Laws&author=C+Wolverton&journal=Sci.+Adv.&volume=4&doi=10.1126%2Fsciadv.aaq1566&pages=eaaq1566&publication_year=2018&)
8. 8.

   Abadi M, Agarwal A, Barham P, Brevdo E, Chen Z et al. 2016.  TensorFlow: large-scale machine learning on heterogeneous distributed systems.  arXiv:1603.04467 [cs]
9. 9.

   Allen FH. 2002.  The Cambridge Structural Database: a quarter of a million crystal structures and rising.  Acta Crystallogr. B 58:380–88

   [[Crossref]](https://doi.org/10.1107/S0108768102003890)
   [[Medline]](https://pubmed.ncbi.nlm.nih.gov/12037359) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000176270700010&DestLinkType=FullRecord&DestApp=WOS_CPL)
   [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=The+Cambridge+Structural+Database%3A+a+quarter+of+a+million+crystal+structures+and+rising&author=FH.+Allen&journal=Acta+Crystallogr.+B&volume=58&doi=10.1107%2FS0108768102003890&pages=380-88&publication_year=2002&)
10. 10.

    Seiler KP, George GA, Happ MP, Bodycombe NE, Carrinski HA et al. 2007.  ChemBank: a small-molecule screening and cheminformatics resource database.  Nucleic Acids Res 36:D351–59

    [[Crossref]](https://doi.org/10.1093/nar/gkm843)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/17947324) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000252545400064&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=ChemBank%3A+a+small-molecule+screening+and+cheminformatics+resource+database&author=KP+Seiler&author=GA+George&author=MP+Happ&author=NE+Bodycombe&author=HA+Carrinski&journal=Nucleic+Acids+Res&volume=36&doi=10.1093%2Fnar%2Fgkm843&pages=D351-59&publication_year=2007&)
11. 11.

    Benson DA, Karsch-Mizrachi I, Lipman DJ, Ostell J, Sayers EW 2008.  GenBank.  Nucleic Acids Res 37:D26–31

    [[Crossref]](https://doi.org/10.1093/nar/gkn723)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000261906200005&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=GenBank&author=DA+Benson&author=I+Karsch-Mizrachi&author=DJ+Lipman&author=J+Ostell&author=EW+Sayers&journal=Nucleic+Acids+Res&volume=37&doi=10.1093%2Fnar%2Fgkn723&pages=D26-31&publication_year=2008&)
12. 12.

    Kim S, Thiessen PA, Bolton EE, Chen J, Fu G et al. 2015.  PubChem substance and compound databases.  Nucleic Acids Res 44:D1202–13

    [[Crossref]](https://doi.org/10.1093/nar/gkv951)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26400175) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000371261700170&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=PubChem+substance+and+compound+databases&author=S+Kim&author=PA+Thiessen&author=EE+Bolton&author=J+Chen&author=G+Fu&journal=Nucleic+Acids+Res&volume=44&doi=10.1093%2Fnar%2Fgkv951&pages=D1202-13&publication_year=2015&)
13. 13.

    Blaiszik B, Chard K, Pruyne J, Ananthakrishnan R, Tuecke S, Foster I 2016.  The materials data facility: data services to advance materials science research.  JOM 68:2045–52

    [[Crossref]](https://doi.org/10.1007/s11837-016-2001-3)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000381991400010&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=The+materials+data+facility%3A+data+services+to+advance+materials+science+research&author=B+Blaiszik&author=K+Chard&author=J+Pruyne&author=R+Ananthakrishnan&author=S+Tuecke&author=I+Foster&journal=JOM&volume=68&doi=10.1007%2Fs11837-016-2001-3&pages=2045-52&publication_year=2016&)
14. 14.

    Draxl C, Scheffler M. 2018.  NOMAD: the FAIR concept for big data–driven materials science.  MRS Bull 43:676–82

    [[Crossref]](https://doi.org/10.1557/mrs.2018.208)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=NOMAD%3A+the+FAIR+concept+for+big+data%E2%80%93driven+materials+science&author=C+Draxl&author=M.+Scheffler&journal=MRS+Bull&volume=43&doi=10.1557%2Fmrs.2018.208&pages=676-82&publication_year=2018&)
15. 15.

    O'Mara J, Meredig B, Michel K 2016.  Materials data infrastructure: a case study of the Citrination platform to examine data import, storage, and access.  JOM 68:2031–34

    [[Crossref]](https://doi.org/10.1007/s11837-016-1984-0)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000381991400008&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+data+infrastructure%3A+a+case+study+of+the+Citrination+platform+to+examine+data+import%2C+storage%2C+and+access&author=J+O%27Mara&author=B+Meredig&author=K+Michel&journal=JOM&volume=68&doi=10.1007%2Fs11837-016-1984-0&pages=2031-34&publication_year=2016&)
16. 16.

    Seshadri R, Sparks TD. 2016.  Perspective: interactive material property databases through aggregation of literature data.  APL Mater 4:053206

    [[Crossref]](https://doi.org/10.1063/1.4944682)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000377720400010&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Perspective%3A+interactive+material+property+databases+through+aggregation+of+literature+data&author=R+Seshadri&author=TD.+Sparks&journal=APL+Mater&volume=4&doi=10.1063%2F1.4944682&pages=053206&publication_year=2016&)
17. 17.

    Rickman J, Chan H, Harmer M, Smeltzer J, Marvel C et al. 2019.  Materials informatics for the screening of multi-principal elements and high-entropy alloys.  Nat. Commun. 10:2618

    [[Crossref]](https://doi.org/10.1038/s41467-019-10533-1)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+informatics+for+the+screening+of+multi-principal+elements+and+high-entropy+alloys&author=J+Rickman&author=H+Chan&author=M+Harmer&author=J+Smeltzer&author=C+Marvel&journal=Nat.+Commun.&volume=10&doi=10.1038%2Fs41467-019-10533-1&pages=2618&publication_year=2019&)
18. 18.

    Iwasaki Y, Takeuchi I, Stanev V, Kusne AG, Ishida M et al. 2019.  Machine-learning guided discovery of a new thermoelectric material.  Sci. Rep. 9:2751

    [[Crossref]](https://doi.org/10.1038/s41598-019-39278-z)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine-learning+guided+discovery+of+a+new+thermoelectric+material&author=Y+Iwasaki&author=I+Takeuchi&author=V+Stanev&author=AG+Kusne&author=M+Ishida&journal=Sci.+Rep.&volume=9&doi=10.1038%2Fs41598-019-39278-z&pages=2751&publication_year=2019&)
19. 19.

    Balachandran PV, Kowalski B, Sehirlioglu A, Lookman T 2018.  Experimental search for high-temperature ferroelectric perovskites guided by two-step machine learning.  Nat. Commun. 9:1668

    [[Crossref]](https://doi.org/10.1038/s41467-018-03821-9)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29700297) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000430922400001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Experimental+search+for+high-temperature+ferroelectric+perovskites+guided+by+two-step+machine+learning&author=PV+Balachandran&author=B+Kowalski&author=A+Sehirlioglu&author=T+Lookman&journal=Nat.+Commun.&volume=9&doi=10.1038%2Fs41467-018-03821-9&pages=1668&publication_year=2018&)
20. 20.

    Min K, Choi B, Park K, Cho E 2018.  Machine learning assisted optimization of electrochemical properties for Ni-rich cathode materials.  Sci. Rep. 8:15778

    [[Crossref]](https://doi.org/10.1038/s41598-018-34201-4)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+assisted+optimization+of+electrochemical+properties+for+Ni-rich+cathode+materials&author=K+Min&author=B+Choi&author=K+Park&author=E+Cho&journal=Sci.+Rep.&volume=8&doi=10.1038%2Fs41598-018-34201-4&pages=15778&publication_year=2018&)
21. 21.

    Hatakeyama-Sato K, Tezuka T, Nishikitani Y, Nishide H, Oyaizu K 2018.  Synthesis of lithium-ion conducting polymers designed by machine learning–based prediction and screening.  Chem. Lett. 48:130–32

    [[Crossref]](https://doi.org/10.1246/cl.180847)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Synthesis+of+lithium-ion+conducting+polymers+designed+by+machine+learning%E2%80%93based+prediction+and+screening&author=K+Hatakeyama-Sato&author=T+Tezuka&author=Y+Nishikitani&author=H+Nishide&author=K+Oyaizu&journal=Chem.+Lett.&volume=48&doi=10.1246%2Fcl.180847&pages=130-32&publication_year=2018&)
22. 22.

    Wen C, Zhang Y, Wang C, Xue D, Bai Y et al. 2019.  Machine learning assisted design of high entropy alloys with desired property.  Acta Mater 170:109–17

    [[Crossref]](https://doi.org/10.1016/j.actamat.2019.03.010)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+assisted+design+of+high+entropy+alloys+with+desired+property&author=C+Wen&author=Y+Zhang&author=C+Wang&author=D+Xue&author=Y+Bai&journal=Acta+Mater&volume=170&doi=10.1016%2Fj.actamat.2019.03.010&pages=109-17&publication_year=2019&)
23. 23.

    Hohenberg P, Kohn W. 1964.  Inhomogeneous electron gas.  Phys. Rev. B 136:864–71

    [[Crossref]](https://doi.org/10.1103/PhysRev.136.B864)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Inhomogeneous+electron+gas&author=P+Hohenberg&author=W.+Kohn&journal=Phys.+Rev.+B&volume=136&doi=10.1103%2FPhysRev.136.B864&pages=864-71&publication_year=1964&)
24. 24.

    Kohn W, Sham LJ. 1965.  Self-consistent equations including exchange and correlation effects.  Phys. Rev. A 140:1133–38

    [[Crossref]](https://doi.org/10.1103/PhysRev.140.A1133)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Self-consistent+equations+including+exchange+and+correlation+effects&author=W+Kohn&author=LJ.+Sham&journal=Phys.+Rev.+A&volume=140&doi=10.1103%2FPhysRev.140.A1133&pages=1133-38&publication_year=1965&)
25. 25.

    Kresse G, Hafner J. 1993.  Ab initio molecular dynamics for liquid metals.  Phys. Rev. B 47:558–61

    [[Crossref]](https://doi.org/10.1103/PhysRevB.47.558)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Ab+initio+molecular+dynamics+for+liquid+metals&author=G+Kresse&author=J.+Hafner&journal=Phys.+Rev.+B&volume=47&doi=10.1103%2FPhysRevB.47.558&pages=558-61&publication_year=1993&)
26. 26.

    Hafner J. 2008.  Ab-initio simulations of materials using VASP: density-functional theory and beyond.  J. Comput. Chem. 29:2044–78

    [[Crossref]](https://doi.org/10.1002/jcc.21057)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/18623101) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000258764600002&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Ab-initio+simulations+of+materials+using+VASP%3A+density-functional+theory+and+beyond&author=J.+Hafner&journal=J.+Comput.+Chem.&volume=29&doi=10.1002%2Fjcc.21057&pages=2044-78&publication_year=2008&)
27. 27.

    Curtarolo S, Setyawan W, Wang S, Xue J, Yang K et al. 2012.  Aflowlib.org: a distributed materials properties repository from high-throughput ab initio calculations.  Comput. Mater. Sci. 58:227–35

    [[Crossref]](https://doi.org/10.1016/j.commatsci.2012.02.002)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000302118400031&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Aflowlib.org%3A+a+distributed+materials+properties+repository+from+high-throughput+ab+initio+calculations&author=S+Curtarolo&author=W+Setyawan&author=S+Wang&author=J+Xue&author=K+Yang&journal=Comput.+Mater.+Sci.&volume=58&doi=10.1016%2Fj.commatsci.2012.02.002&pages=227-35&publication_year=2012&)
28. 28.

    Jain A, Ong SP, Hautier G, Chen W, Richards WD et al. 2013.  Commentary: The materials project: a materials genome approach to accelerating materials innovation.  APL Mater 1:011002

    [[Crossref]](https://doi.org/10.1063/1.4812323)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000332272300003&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Commentary%3A+The+materials+project%3A+a+materials+genome+approach+to+accelerating+materials+innovation&author=A+Jain&author=SP+Ong&author=G+Hautier&author=W+Chen&author=WD+Richards&journal=APL+Mater&volume=1&doi=10.1063%2F1.4812323&pages=011002&publication_year=2013&)
29. 29.

    Saal JE, Kirklin S, Aykol M, Meredig B, Wolverton C 2013.  Materials design and discovery with high-throughput density functional theory: the Open Quantum Materials Database (OQMD).  JOM 65:1501–9

    [[Crossref]](https://doi.org/10.1007/s11837-013-0755-4)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000327496400020&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Materials+design+and+discovery+with+high-throughput+density+functional+theory%3A+the+Open+Quantum+Materials+Database+%28OQMD%29&author=JE+Saal&author=S+Kirklin&author=M+Aykol&author=B+Meredig&author=C+Wolverton&journal=JOM&volume=65&doi=10.1007%2Fs11837-013-0755-4&pages=1501-9&publication_year=2013&)
30. 30.

    Ward L, Aykol M, Blaiszik B, Foster I, Meredig B et al. 2018.  Strategies for accelerating the adoption of materials informatics.  MRS Bull 43:683–89

    [[Crossref]](https://doi.org/10.1557/mrs.2018.204)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Strategies+for+accelerating+the+adoption+of+materials+informatics&author=L+Ward&author=M+Aykol&author=B+Blaiszik&author=I+Foster&author=B+Meredig&journal=MRS+Bull&volume=43&doi=10.1557%2Fmrs.2018.204&pages=683-89&publication_year=2018&)
31. 31.

    Mansouri Tehrani A, Oliynyk AO, Parry M, Rizvi Z, Couper S et al. 2018.  Machine learning directed search for ultraincompressible, superhard materials.  J. Am. Chem. Soc. 140:9844–53

    [[Crossref]](https://doi.org/10.1021/jacs.8b02717)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+directed+search+for+ultraincompressible%2C+superhard+materials&author=A+Mansouri+Tehrani&author=AO+Oliynyk&author=M+Parry&author=Z+Rizvi&author=S+Couper&journal=J.+Am.+Chem.+Soc.&volume=140&doi=10.1021%2Fjacs.8b02717&pages=9844-53&publication_year=2018&)
32. 32.

    Zhuo Y, Mansouri Tehrani A, Oliynyk AO, Duke AC, Brgoch J 2018.  Identifying an efficient, thermally robust inorganic phosphor host via machine learning.  Nat. Commun. 9:4377

    [[Crossref]](https://doi.org/10.1038/s41467-018-06625-z)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Identifying+an+efficient%2C+thermally+robust+inorganic+phosphor+host+via+machine+learning&author=Y+Zhuo&author=A+Mansouri+Tehrani&author=AO+Oliynyk&author=AC+Duke&author=J+Brgoch&journal=Nat.+Commun.&volume=9&doi=10.1038%2Fs41467-018-06625-z&pages=4377&publication_year=2018&)
33. 33.

    Bassman L, Rajak P, Kalia RK, Nakano A, Sha F et al. 2018.  Active learning for accelerated design of layered materials.  npj Comput. Mater. 4:74

    [[Crossref]](https://doi.org/10.1038/s41524-018-0129-0)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Active+learning+for+accelerated+design+of+layered+materials&author=L+Bassman&author=P+Rajak&author=RK+Kalia&author=A+Nakano&author=F+Sha&journal=npj+Comput.+Mater.&volume=4&doi=10.1038%2Fs41524-018-0129-0&pages=74&publication_year=2018&)
34. 34.

    Huo H, Rupp M. 2017.  Unified representation for machine learning of molecules and crystals.  arXiv:1704.06439 [physics.chem-ph]
35. 35.

    Askerka M, Li Z, Lempen M, Liu Y, Johnston A et al. 2019.  Learning-in-templates enables accelerated discovery and synthesis of new stable double perovskites.  J. Am. Chem. Soc. 141:3682–90

    [[Crossref]](https://doi.org/10.1021/jacs.8b13420)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Learning-in-templates+enables+accelerated+discovery+and+synthesis+of+new+stable+double+perovskites&author=M+Askerka&author=Z+Li&author=M+Lempen&author=Y+Liu&author=A+Johnston&journal=J.+Am.+Chem.+Soc.&volume=141&doi=10.1021%2Fjacs.8b13420&pages=3682-90&publication_year=2019&)
36. 36.

    Schütt K, Glawe H, Brockherde F, Sanna A, Müller K, Gross E 2014.  How to represent crystal structures for machine learning: towards fast prediction of electronic properties.  Phys. Rev. B 89:205118

    [[Crossref]](https://doi.org/10.1103/PhysRevB.89.205118)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000336248300003&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=How+to+represent+crystal+structures+for+machine+learning%3A+towards+fast+prediction+of+electronic+properties&author=K+Sch%C3%BCtt&author=H+Glawe&author=F+Brockherde&author=A+Sanna&author=K+M%C3%BCller&author=E+Gross&journal=Phys.+Rev.+B&volume=89&doi=10.1103%2FPhysRevB.89.205118&pages=205118&publication_year=2014&)
37. 37.

    Ward L, Dunn A, Faghaninia A, Zimmermann NE, Bajaj S et al. 2018.  Matminer: an open source toolkit for materials data mining.  Comput. Mater. Sci. 152:60–69

    [[Crossref]](https://doi.org/10.1016/j.commatsci.2018.05.018)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Matminer%3A+an+open+source+toolkit+for+materials+data+mining&author=L+Ward&author=A+Dunn&author=A+Faghaninia&author=NE+Zimmermann&author=S+Bajaj&journal=Comput.+Mater.+Sci.&volume=152&doi=10.1016%2Fj.commatsci.2018.05.018&pages=60-69&publication_year=2018&)
38. 38.

    Faber FA, Christensen AS, Huang B, von Lilienfeld OA 2018.  Alchemical and structural distribution based representation for universal quantum machine learning.  J. Chem. Phys. 148:241717

    [[Crossref]](https://doi.org/10.1063/1.5020710)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29960351) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000437190300020&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Alchemical+and+structural+distribution+based+representation+for+universal+quantum+machine+learning&author=FA+Faber&author=AS+Christensen&author=B+Huang&author=OA+von+Lilienfeld&journal=J.+Chem.+Phys.&volume=148&doi=10.1063%2F1.5020710&pages=241717&publication_year=2018&)
39. 39.

    Ward L, Liu R, Krishna A, Hegde VI, Agrawal A et al. 2017.  Including crystal structure attributes in machine learning models of formation energies via Voronoi tessellations.  Phys. Rev. B 96:024104

    [[Crossref]](https://doi.org/10.1103/PhysRevB.96.024104)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000405509100001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Including+crystal+structure+attributes+in+machine+learning+models+of+formation+energies+via+Voronoi+tessellations&author=L+Ward&author=R+Liu&author=A+Krishna&author=VI+Hegde&author=A+Agrawal&journal=Phys.+Rev.+B&volume=96&doi=10.1103%2FPhysRevB.96.024104&pages=024104&publication_year=2017&)
40. 40.

    Ward L, Agrawal A, Choudhary A, Wolverton C 2016.  A general-purpose machine learning framework for predicting properties of inorganic materials.  npj Comput. Mater. 2:16028

    [[Crossref]](https://doi.org/10.1038/npjcompumats.2016.28)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426821500024&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=A+general-purpose+machine+learning+framework+for+predicting+properties+of+inorganic+materials&author=L+Ward&author=A+Agrawal&author=A+Choudhary&author=C+Wolverton&journal=npj+Comput.+Mater.&volume=2&doi=10.1038%2Fnpjcompumats.2016.28&pages=16028&publication_year=2016&)
41. 41.

    Rosenbrock CW, Homer ER, Csányi G, Hart GL 2017.  Discovering the building blocks of atomic systems using machine learning: application to grain boundaries.  npj Comput. Mater. 3:29

    [[Crossref]](https://doi.org/10.1038/s41524-017-0027-x)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426833500001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Discovering+the+building+blocks+of+atomic+systems+using+machine+learning%3A+application+to+grain+boundaries&author=CW+Rosenbrock&author=ER+Homer&author=G+Cs%C3%A1nyi&author=GL+Hart&journal=npj+Comput.+Mater.&volume=3&doi=10.1038%2Fs41524-017-0027-x&pages=29&publication_year=2017&)
42. 42.

    Gomberg JA, Medford AJ, Kalidindi SR 2017.  Extracting knowledge from molecular mechanics simulations of grain boundaries using machine learning.  Acta Mater 133:100–8

    [[Crossref]](https://doi.org/10.1016/j.actamat.2017.05.009)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000407413100011&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Extracting+knowledge+from+molecular+mechanics+simulations+of+grain+boundaries+using+machine+learning&author=JA+Gomberg&author=AJ+Medford&author=SR+Kalidindi&journal=Acta+Mater&volume=133&doi=10.1016%2Fj.actamat.2017.05.009&pages=100-8&publication_year=2017&)
43. 43.

    Gilmer J, Schoenholz SS, Riley PF, Vinyals O, Dahl GE 2017.  Neural message passing for quantum chemistry.  Proceedings of the 34th International Conference on Machine Learning D Precup, YW Teh 1263–72 New York: ACM <https://dl.acm.org/doi/10.5555/3305381.3305512>


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Neural+message+passing+for+quantum+chemistry&author=J+Gilmer&author=SS+Schoenholz&author=PF+Riley&author=O+Vinyals&author=GE+Dahl&journal=Proceedings+of+the+34th+International+Conference+on+Machine+Learning&pages=1263-72&publication_year=2017&)
44. 44.

    Schütt KT, Sauceda HE, Kindermans PJ, Tkatchenko A, Müller KR 2018.  SchNet—a deep learning architecture for molecules and materials.  J. Chem. Phys. 148:241722

    [[Crossref]](https://doi.org/10.1063/1.5019779)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29960322) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000437190300025&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=SchNet%E2%80%94a+deep+learning+architecture+for+molecules+and+materials&author=KT+Sch%C3%BCtt&author=HE+Sauceda&author=PJ+Kindermans&author=A+Tkatchenko&author=KR+M%C3%BCller&journal=J.+Chem.+Phys.&volume=148&doi=10.1063%2F1.5019779&pages=241722&publication_year=2018&)
45. 45.

    Xie T, Grossman JC. 2018.  Crystal graph convolutional neural networks for an accurate and interpretable prediction of material properties.  Phys. Rev. Lett. 120:145301

    [[Crossref]](https://doi.org/10.1103/PhysRevLett.120.145301)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29694125) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000429451000012&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Crystal+graph+convolutional+neural+networks+for+an+accurate+and+interpretable+prediction+of+material+properties&author=T+Xie&author=JC.+Grossman&journal=Phys.+Rev.+Lett.&volume=120&doi=10.1103%2FPhysRevLett.120.145301&pages=145301&publication_year=2018&)
46. 46.

    Bartók AP, De S, Poelking C, Bernstein N, Kermode JR et al. 2017.  Machine learning unifies the modeling of materials and molecules.  Sci. Adv. 3:e1701816

    [[Crossref]](https://doi.org/10.1126/sciadv.1701816)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29242828) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000418003100020&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+unifies+the+modeling+of+materials+and+molecules&author=AP+Bart%C3%B3k&author=S+De&author=C+Poelking&author=N+Bernstein&author=JR+Kermode&journal=Sci.+Adv.&volume=3&doi=10.1126%2Fsciadv.1701816&pages=e1701816&publication_year=2017&)
47. 47.

    Hall MA. 1999. Correlation-based feature selection for machine learning PhD Thesis, Univ. Waikato Hamilton, N. Z:.


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Correlation-based+feature+selection+for+machine+learning&author=MA.+Hall&publication_year=1999&)
48. 48.

    Jolliffe IT, Cadima J. 2016.  Principal component analysis: a review and recent developments.  Philos. Trans. R. Soc. A 374:20150202

    [[Crossref]](https://doi.org/10.1098/rsta.2015.0202)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26953178) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000372553500008&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Principal+component+analysis%3A+a+review+and+recent+developments&author=IT+Jolliffe&author=J.+Cadima&journal=Philos.+Trans.+R.+Soc.+A&volume=374&doi=10.1098%2Frsta.2015.0202&pages=20150202&publication_year=2016&)
49. 49.

    Sinkov NA, Harynuk JJ. 2011.  Cluster resolution: a metric for automated, objective and optimized feature selection in chemometric modeling.  Talanta 83:1079–87

    [[Crossref]](https://doi.org/10.1016/j.talanta.2010.10.025)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/21215842) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000286718700004&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Cluster+resolution%3A+a+metric+for+automated%2C+objective+and+optimized+feature+selection+in+chemometric+modeling&author=NA+Sinkov&author=JJ.+Harynuk&journal=Talanta&volume=83&doi=10.1016%2Fj.talanta.2010.10.025&pages=1079-87&publication_year=2011&)
50. 50.

    Meredig B, Antono E, Church C, Hutchinson M, Ling J et al. 2018.  Can machine learning identify the next high-temperature superconductor? Examining extrapolation performance for materials discovery.  Mol. Syst. Des. Eng. 3:819–25

    [[Crossref]](https://doi.org/10.1039/C8ME00012C)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Can+machine+learning+identify+the+next+high-temperature+superconductor%3F+Examining+extrapolation+performance+for+materials+discovery&author=B+Meredig&author=E+Antono&author=C+Church&author=M+Hutchinson&author=J+Ling&journal=Mol.+Syst.+Des.+Eng.&volume=3&doi=10.1039%2FC8ME00012C&pages=819-25&publication_year=2018&)
51. 51.

    Lu HJ, Zou N, Jacobs R, Afflerbach B, Lu XG, Morgan D 2019.  Error assessment and optimal cross-validation approaches in machine learning applied to impurity diffusion.  Comput. Mater. Sci. 169:109075

    [[Crossref]](https://doi.org/10.1016/j.commatsci.2019.06.010)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Error+assessment+and+optimal+cross-validation+approaches+in+machine+learning+applied+to+impurity+diffusion&author=HJ+Lu&author=N+Zou&author=R+Jacobs&author=B+Afflerbach&author=XG+Lu&author=D+Morgan&journal=Comput.+Mater.+Sci.&volume=169&doi=10.1016%2Fj.commatsci.2019.06.010&pages=109075&publication_year=2019&)
52. 52.

    Sheridan RP. 2013.  Time-split cross-validation as a method for estimating the goodness of prospective prediction.  J. Chem. Inf. Model. 53:783–90

    [[Crossref]](https://doi.org/10.1021/ci400084k)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/23521722) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000318060200006&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Time-split+cross-validation+as+a+method+for+estimating+the+goodness+of+prospective+prediction&author=RP.+Sheridan&journal=J.+Chem.+Inf.+Model.&volume=53&doi=10.1021%2Fci400084k&pages=783-90&publication_year=2013&)
53. 53.

    Wallach I, Heifets A. 2018.  Most ligand-based classification benchmarks reward memorization rather than generalization.  J. Chem. Inf. Model. 58:916–32

    [[Crossref]](https://doi.org/10.1021/acs.jcim.7b00403)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29698607) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000433634900004&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Most+ligand-based+classification+benchmarks+reward+memorization+rather+than+generalization&author=I+Wallach&author=A.+Heifets&journal=J.+Chem.+Inf.+Model.&volume=58&doi=10.1021%2Facs.jcim.7b00403&pages=916-32&publication_year=2018&)
54. 54.

    Riley P. 2019.  Three pitfalls to avoid in machine learning.  Nature 572:27–29

    [[Crossref]](https://doi.org/10.1038/d41586-019-02307-y)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Three+pitfalls+to+avoid+in+machine+learning&author=P.+Riley&journal=Nature&volume=572&doi=10.1038%2Fd41586-019-02307-y&pages=27-29&publication_year=2019&)
55. 55.

    Vapnik VN. 1999.  An overview of statistical learning theory.  IEEE Trans. Neural Netw. 10:988–99

    [[Crossref]](https://doi.org/10.1109/72.788640)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=An+overview+of+statistical+learning+theory&author=VN.+Vapnik&journal=IEEE+Trans.+Neural+Netw.&volume=10&doi=10.1109%2F72.788640&pages=988-99&publication_year=1999&)
56. 56.

    Stanev V, Oses C, Kusne AG, Rodriguez E, Paglione J et al. 2018.  Machine learning modeling of superconducting critical temperature.  npj Comput. Mater. 4:29

    [[Crossref]](https://doi.org/10.1038/s41524-018-0085-8)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000438373200001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+modeling+of+superconducting+critical+temperature&author=V+Stanev&author=C+Oses&author=AG+Kusne&author=E+Rodriguez&author=J+Paglione&journal=npj+Comput.+Mater.&volume=4&doi=10.1038%2Fs41524-018-0085-8&pages=29&publication_year=2018&)
57. 57.

    Ling J, Hutchinson M, Antono E, Paradiso S, Meredig B 2017.  High-dimensional materials and process optimization using data-driven experimental design with well-calibrated uncertainty estimates.  Integr. Mater. Manuf. Innov. 6:207–17

    [[Crossref]](https://doi.org/10.1007/s40192-017-0098-z)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000411716600001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=High-dimensional+materials+and+process+optimization+using+data-driven+experimental+design+with+well-calibrated+uncertainty+estimates&author=J+Ling&author=M+Hutchinson&author=E+Antono&author=S+Paradiso&author=B+Meredig&journal=Integr.+Mater.+Manuf.+Innov.&volume=6&doi=10.1007%2Fs40192-017-0098-z&pages=207-17&publication_year=2017&)
58. 58.

    De Jong M, Chen W, Angsten T, Jain A, Notestine R et al. 2015.  Charting the complete elastic properties of inorganic crystalline compounds.  Sci. Data 2:150009

    [[Crossref]](https://doi.org/10.1038/sdata.2015.9)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/25984348) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000390328900001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Charting+the+complete+elastic+properties+of+inorganic+crystalline+compounds&author=M+De+Jong&author=W+Chen&author=T+Angsten&author=A+Jain&author=R+Notestine&journal=Sci.+Data&volume=2&doi=10.1038%2Fsdata.2015.9&pages=150009&publication_year=2015&)
59. 59.

    Breiman L. 2001.  Random forests.  Mach. Learn. 45:5–32

    [[Crossref]](https://doi.org/10.1023/A:1010933404324)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Random+forests&author=L.+Breiman&journal=Mach.+Learn.&volume=45&doi=10.1023%2FA%3A1010933404324&pages=5-32&publication_year=2001&)
60. 60.

    Wager S, Hastie T, Efron B 2014.  Confidence intervals for random forests: the jackknife and the infinitesimal jackknife.  J. Mach. Learn. Res. 15:1625–51


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Confidence+intervals+for+random+forests%3A+the+jackknife+and+the+infinitesimal+jackknife&author=S+Wager&author=T+Hastie&author=B+Efron&journal=J.+Mach.+Learn.+Res.&volume=15&pages=1625-51&publication_year=2014&)
61. 61.

    Krogh A, Vedelsby J. 1996.  Neural network ensembles, cross validation, and active learning.  Advances in Neural Information Processing Systems 8 (NIPS 1995) DS Touretzky, MC Mozer, ME Hasselmo 231–38 Cambridge, MA: MIT Press


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Neural+network+ensembles%2C+cross+validation%2C+and+active+learning&author=A+Krogh&author=J.+Vedelsby&journal=Advances+in+Neural+Information+Processing+Systems+8+%28NIPS+1995%29&pages=231-38&publication_year=1996&)
62. 62.

    LeCun Y, Bengio Y, Hinton G 2015.  Deep learning.  Nature 521:436–44

    [[Crossref]](https://doi.org/10.1038/nature14539)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26017442) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000355286600030&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Deep+learning&author=Y+LeCun&author=Y+Bengio&author=G+Hinton&journal=Nature&volume=521&doi=10.1038%2Fnature14539&pages=436-44&publication_year=2015&)
63. 63.

    Kim K, Kang S, Yoo J, Kwon Y, Nam Y et al. 2018.  Deep-learning-based inverse design model for intelligent discovery of organic molecules.  npj Comput. Mater. 4:67

    [[Crossref]](https://doi.org/10.1038/s41524-018-0128-1)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Deep-learning-based+inverse+design+model+for+intelligent+discovery+of+organic+molecules&author=K+Kim&author=S+Kang&author=J+Yoo&author=Y+Kwon&author=Y+Nam&journal=npj+Comput.+Mater.&volume=4&doi=10.1038%2Fs41524-018-0128-1&pages=67&publication_year=2018&)
64. 64.

    Gómez-Bombarelli R, Aguilera-Iparraguirre J, Hirzel TD, Duvenaud D, Maclaurin D et al. 2016.  Design of efficient molecular organic light-emitting diodes by a high-throughput virtual screening and experimental approach.  Nat. Mater. 15:1120–27

    [[Crossref]](https://doi.org/10.1038/nmat4717)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Design+of+efficient+molecular+organic+light-emitting+diodes+by+a+high-throughput+virtual+screening+and+experimental+approach&author=R+G%C3%B3mez-Bombarelli&author=J+Aguilera-Iparraguirre&author=TD+Hirzel&author=D+Duvenaud&author=D+Maclaurin&journal=Nat.+Mater.&volume=15&doi=10.1038%2Fnmat4717&pages=1120-27&publication_year=2016&)
65. 65.

    Oliynyk AO, Antono E, Sparks TD, Ghadbeigi L, Gaultois MW et al. 2016.  High-throughput machine-learning-driven synthesis of full-Heusler compounds.  Chem. Mater. 28:7324–31

    [[Crossref]](https://doi.org/10.1021/acs.chemmater.6b02724)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000386421900018&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=High-throughput+machine-learning-driven+synthesis+of+full-Heusler+compounds&author=AO+Oliynyk&author=E+Antono&author=TD+Sparks&author=L+Ghadbeigi&author=MW+Gaultois&journal=Chem.+Mater.&volume=28&doi=10.1021%2Facs.chemmater.6b02724&pages=7324-31&publication_year=2016&)
66. 66.

    Agrawal A, Deshpande PD, Cecen A, Basavarsu GP, Choudhary AN, Kalidindi SR 2014.  Exploration of data science techniques to predict fatigue strength of steel from composition and processing parameters.  Integr. Mater. Manuf. Innov. 3:90–108

    [[Crossref]](https://doi.org/10.1186/2193-9772-3-8)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Exploration+of+data+science+techniques+to+predict+fatigue+strength+of+steel+from+composition+and+processing+parameters&author=A+Agrawal&author=PD+Deshpande&author=A+Cecen&author=GP+Basavarsu&author=AN+Choudhary&author=SR+Kalidindi&journal=Integr.+Mater.+Manuf.+Innov.&volume=3&doi=10.1186%2F2193-9772-3-8&pages=90-108&publication_year=2014&)
67. 67.

    Iwasaki Y, Sawada R, Stanev V, Ishida M, Kirihara A et al. 2019.  Materials development by interpretable machine learning.  arXiv:1903.02175 [cond-mat.mtrl-sci]
68. 68.

    Xue D, Xue D, Yuan R, Zhou Y, Balachandran PV et al. 2017.  An informatics approach to transformation temperatures of NiTi-based shape memory alloys.  Acta Mater 125:532–41

    [[Crossref]](https://doi.org/10.1016/j.actamat.2016.12.009)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000394201500054&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=An+informatics+approach+to+transformation+temperatures+of+NiTi-based+shape+memory+alloys&author=D+Xue&author=D+Xue&author=R+Yuan&author=Y+Zhou&author=PV+Balachandran&journal=Acta+Mater&volume=125&doi=10.1016%2Fj.actamat.2016.12.009&pages=532-41&publication_year=2017&)
69. 69.

    Hassabis D. 2017.  Artificial intelligence: chess match of the century.  Nature 544:413–14

    [[Crossref]](https://doi.org/10.1038/544413a)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000400051900019&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Artificial+intelligence%3A+chess+match+of+the+century&author=D.+Hassabis&journal=Nature&volume=544&doi=10.1038%2F544413a&pages=413-14&publication_year=2017&)
70. 70.

    Meredig B, Agrawal A, Kirklin S, Saal JE, Doak J et al. 2014.  Combinatorial screening for new materials in unconstrained composition space with machine learning.  Phys. Rev. B 89:094104

    [[Crossref]](https://doi.org/10.1103/PhysRevB.89.094104)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000332759000001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Combinatorial+screening+for+new+materials+in+unconstrained+composition+space+with+machine+learning&author=B+Meredig&author=A+Agrawal&author=S+Kirklin&author=JE+Saal&author=J+Doak&journal=Phys.+Rev.+B&volume=89&doi=10.1103%2FPhysRevB.89.094104&pages=094104&publication_year=2014&)
71. 71.

    Zeier WG, Anand S, Huang L, He R, Zhang H et al. 2017.  Using the 18-electron rule to understand the nominal 19-electron half-Heusler NbCoSb with Nb vacancies.  Chem. Mater. 29:1210–17

    [[Crossref]](https://doi.org/10.1021/acs.chemmater.6b04583)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000394924100039&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Using+the+18-electron+rule+to+understand+the+nominal+19-electron+half-Heusler+NbCoSb+with+Nb+vacancies&author=WG+Zeier&author=S+Anand&author=L+Huang&author=R+He&author=H+Zhang&journal=Chem.+Mater.&volume=29&doi=10.1021%2Facs.chemmater.6b04583&pages=1210-17&publication_year=2017&)
72. 72.

    Hutchinson ML, Antono E, Gibbons BM, Paradiso S, Ling J, Meredig B 2017.  Overcoming data scarcity with transfer learning.  arXiv:1711.05099 [cs.LG]
73. 73.

    De S, Bartók AP, Csányi G, Ceriotti M 2016.  Comparing molecules and solids across structural and alchemical space.  Phys. Chem. Chem. Phys. 18:13754–69

    [[Crossref]](https://doi.org/10.1039/C6CP00415F)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Comparing+molecules+and+solids+across+structural+and+alchemical+space&author=S+De&author=AP+Bart%C3%B3k&author=G+Cs%C3%A1nyi&author=M+Ceriotti&journal=Phys.+Chem.+Chem.+Phys.&volume=18&doi=10.1039%2FC6CP00415F&pages=13754-69&publication_year=2016&)
74. 74.

    Liu AY, Cohen ML. 1989.  Prediction of new low compressibility solids.  Science 245:841–42

    [[Crossref]](https://doi.org/10.1126/science.245.4920.841)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Prediction+of+new+low+compressibility+solids&author=AY+Liu&author=ML.+Cohen&journal=Science&volume=245&doi=10.1126%2Fscience.245.4920.841&pages=841-42&publication_year=1989&)
75. 75.

    Menon A, Childs CM, Poczós B, Washburn NR, Kurtis KE 2019.  Molecular engineering of superplasticizers for metakaolin-portland cement blends with hierarchical machine learning.  Adv. Theory Simul. 2:1800164

    [[Crossref]](https://doi.org/10.1002/adts.201800164)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Molecular+engineering+of+superplasticizers+for+metakaolin-portland+cement+blends+with+hierarchical+machine+learning&author=A+Menon&author=CM+Childs&author=B+Pocz%C3%B3s&author=NR+Washburn&author=KE+Kurtis&journal=Adv.+Theory+Simul.&volume=2&doi=10.1002%2Fadts.201800164&pages=1800164&publication_year=2019&)
76. 76.

    Santosa F, Symes WW. 1986.  Linear inversion of band-limited reflection seismograms.  SIAM J. Sci. Stat. Comput. 7:1307–30

    [[Crossref]](https://doi.org/10.1137/0907087)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Linear+inversion+of+band-limited+reflection+seismograms&author=F+Santosa&author=WW.+Symes&journal=SIAM+J.+Sci.+Stat.+Comput.&volume=7&doi=10.1137%2F0907087&pages=1307-30&publication_year=1986&)
77. 77.

    Bucior BJ, Bobbitt NS, Islamoglu T, Goswami S, Gopalan A et al. 2019.  Energy-based descriptors to rapidly predict hydrogen storage in metal–organic frameworks.  Mol. Syst. Des. Eng. 4:162–74

    [[Crossref]](https://doi.org/10.1039/C8ME00050F)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Energy-based+descriptors+to+rapidly+predict+hydrogen+storage+in+metal%E2%80%93organic+frameworks&author=BJ+Bucior&author=NS+Bobbitt&author=T+Islamoglu&author=S+Goswami&author=A+Gopalan&journal=Mol.+Syst.+Des.+Eng.&volume=4&doi=10.1039%2FC8ME00050F&pages=162-74&publication_year=2019&)
78. 78.

    Raccuglia P, Elbert KC, Adler PD, Falk C, Wenny MB et al. 2016.  Machine-learning-assisted materials discovery using failed experiments.  Nature 533:73–76

    [[Crossref]](https://doi.org/10.1038/nature17439)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/27147027) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000375473900041&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine-learning-assisted+materials+discovery+using+failed+experiments&author=P+Raccuglia&author=KC+Elbert&author=PD+Adler&author=C+Falk&author=MB+Wenny&journal=Nature&volume=533&doi=10.1038%2Fnature17439&pages=73-76&publication_year=2016&)
79. 79.

    Kawazoe Y, Yu J-Z, Tsai A-P, Masumoto T 1997. Phase Diagrams and Physical Properties of Nonequilibrium Alloys, Subvol. A: Nonequilibrium Phase Diagrams of Ternary Amorphous Alloys Landolt–Börnstein Numer. Data Funct. Relatsh. Sci. Technol. 37 Berlin/Heidelberg/New York: Springer


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Phase+Diagrams+and+Physical+Properties+of+Nonequilibrium+Alloys%2C+Subvol.+A%3A+Nonequilibrium+Phase+Diagrams+of+Ternary+Amorphous+Alloys&author=Y+Kawazoe&author=J-Z+Yu&author=A-P+Tsai&author=T+Masumoto&publication_year=1997&)
80. 80.

    Sakurai A, Yada K, Simomura T, Ju S, Kashiwagi M et al. 2019.  Ultranarrow-band wavelength-selective thermal emission with aperiodic multilayered metamaterials designed by Bayesian optimization.  ACS Cent. Sci. 5:319–26

    [[Crossref]](https://doi.org/10.1021/acscentsci.8b00802)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Ultranarrow-band+wavelength-selective+thermal+emission+with+aperiodic+multilayered+metamaterials+designed+by+Bayesian+optimization&author=A+Sakurai&author=K+Yada&author=T+Simomura&author=S+Ju&author=M+Kashiwagi&journal=ACS+Cent.+Sci.&volume=5&doi=10.1021%2Facscentsci.8b00802&pages=319-26&publication_year=2019&)
81. 81.

    Sendek AD, Yang Q, Cubuk ED, Duerloo KAN, Cui Y, Reed EJ 2017.  Holistic computational structure screening of more than 12,000 candidates for solid lithium-ion conductor materials.  Energy Environ. Sci. 10:306–20

    [[Crossref]](https://doi.org/10.1039/C6EE02697D)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Holistic+computational+structure+screening+of+more+than+12%2C000+candidates+for+solid+lithium-ion+conductor+materials&author=AD+Sendek&author=Q+Yang&author=ED+Cubuk&author=KAN+Duerloo&author=Y+Cui&author=EJ+Reed&journal=Energy+Environ.+Sci.&volume=10&doi=10.1039%2FC6EE02697D&pages=306-20&publication_year=2017&)
82. 82.

    Sendek AD, Antoniuk ER, Cubuk ED, Francisco BE, Buettner-Garrett J et al. 2019.  A new solid Li-ion electrolyte from the crystalline lithium-boron-sulfur system.  SSRN Electron. J. <https://dx.doi.org/10.2139/ssrn.3404263>

    [[Crossref]](https://doi.org/10.2139/ssrn.3404263)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=A+new+solid+Li-ion+electrolyte+from+the+crystalline+lithium-boron-sulfur+system&author=AD+Sendek&author=ER+Antoniuk&author=ED+Cubuk&author=BE+Francisco&author=J+Buettner-Garrett&journal=SSRN+Electron.+J.&doi=10.2139%2Fssrn.3404263&publication_year=2019&)
83. 83.

    Häse F, Roch LM, Aspuru-Guzik A 2018.  Chimera: enabling hierarchy based multi-objective optimization for self-driving laboratories.  Chem. Sci. 9:7642–55

    [[Crossref]](https://doi.org/10.1039/C8SC02239A)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Chimera%3A+enabling+hierarchy+based+multi-objective+optimization+for+self-driving+laboratories&author=F+H%C3%A4se&author=LM+Roch&author=A+Aspuru-Guzik&journal=Chem.+Sci.&volume=9&doi=10.1039%2FC8SC02239A&pages=7642-55&publication_year=2018&)
84. 84.

    Solomou A, Zhao G, Boluki S, Joy JK, Qian X et al. 2018.  Multi-objective Bayesian materials discovery: application on the discovery of precipitation strengthened NiTi shape memory alloys through micromechanical modeling.  Mater. Des. 160:810–27

    [[Crossref]](https://doi.org/10.1016/j.matdes.2018.10.014)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Multi-objective+Bayesian+materials+discovery%3A+application+on+the+discovery+of+precipitation+strengthened+NiTi+shape+memory+alloys+through+micromechanical+modeling&author=A+Solomou&author=G+Zhao&author=S+Boluki&author=JK+Joy&author=X+Qian&journal=Mater.+Des.&volume=160&doi=10.1016%2Fj.matdes.2018.10.014&pages=810-27&publication_year=2018&)
85. 85.

    Kingma DP, Welling M. 2013.  Auto-encoding variational Bayes.  arXiv:1312.6114 [stat.ML]
86. 86.

    Gómez-Bombarelli R, Wei JN, Duvenaud D, Hernández-Lobato JM, Sánchez-Lengeling B et al. 2018.  Automatic chemical design using a data-driven continuous representation of molecules.  ACS Cent. Sci. 4:268–76

    [[Crossref]](https://doi.org/10.1021/acscentsci.7b00572)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29532027) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426613700019&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Automatic+chemical+design+using+a+data-driven+continuous+representation+of+molecules&author=R+G%C3%B3mez-Bombarelli&author=JN+Wei&author=D+Duvenaud&author=JM+Hern%C3%A1ndez-Lobato&author=B+S%C3%A1nchez-Lengeling&journal=ACS+Cent.+Sci.&volume=4&doi=10.1021%2Facscentsci.7b00572&pages=268-76&publication_year=2018&)
87. 87.

    Goodfellow I, Pouget-Abadie J, Mirza M, Xu B, Warde-Farley D et al. 2014.  Generative adversarial nets.  Advances in Neural Information Processing Systems 27 (NIPS 2014) Z Ghahramani, M Welling, C Cortes, ND Lawrence, KQ Weinberger San Diego: Neural Inf. Process. Syst.


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Generative+adversarial+nets&author=I+Goodfellow&author=J+Pouget-Abadie&author=M+Mirza&author=B+Xu&author=D+Warde-Farley&journal=Advances+in+Neural+Information+Processing+Systems+27+%28NIPS+2014%29&publication_year=2014&)
88. 88.

    Nikolaev P, Hooper D, Webber F, Rao R, Decker K et al. 2016.  Autonomy in materials research: a case study in carbon nanotube growth.  npj Comput. Mater. 2:16031

    [[Crossref]](https://doi.org/10.1038/npjcompumats.2016.31)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000426821500026&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Autonomy+in+materials+research%3A+a+case+study+in+carbon+nanotube+growth&author=P+Nikolaev&author=D+Hooper&author=F+Webber&author=R+Rao&author=K+Decker&journal=npj+Comput.+Mater.&volume=2&doi=10.1038%2Fnpjcompumats.2016.31&pages=16031&publication_year=2016&)
89. 89.

    Holm EA. 2019.  In defense of the black box.  Science 364:26–27

    [[Crossref]](https://doi.org/10.1126/science.aax0162)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=In+defense+of+the+black+box&author=EA.+Holm&journal=Science&volume=364&doi=10.1126%2Fscience.aax0162&pages=26-27&publication_year=2019&)
90. 90.

    Mannodi-Kanakkithodi A, Pilania G, Huan TD, Lookman T, Ramprasad R 2016.  Machine learning strategy for accelerated design of polymer dielectrics.  Sci. Rep. 6:20952

    [[Crossref]](https://doi.org/10.1038/srep20952)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/26876223) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000370055400001&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine+learning+strategy+for+accelerated+design+of+polymer+dielectrics&author=A+Mannodi-Kanakkithodi&author=G+Pilania&author=TD+Huan&author=T+Lookman&author=R+Ramprasad&journal=Sci.+Rep.&volume=6&doi=10.1038%2Fsrep20952&pages=20952&publication_year=2016&)
91. 91.

    Oliynyk AO, Adutwum LA, Harynuk JJ, Mar A 2016.  Classifying crystal structures of binary compounds AB through cluster resolution feature selection and support vector machine analysis.  Chem. Mater. 28:6672–81

    [[Crossref]](https://doi.org/10.1021/acs.chemmater.6b02905)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000384399000033&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Classifying+crystal+structures+of+binary+compounds+AB+through+cluster+resolution+feature+selection+and+support+vector+machine+analysis&author=AO+Oliynyk&author=LA+Adutwum&author=JJ+Harynuk&author=A+Mar&journal=Chem.+Mater.&volume=28&doi=10.1021%2Facs.chemmater.6b02905&pages=6672-81&publication_year=2016&)
92. 92.

    Villars P 2007. Pearson's Crystal Data®: crystal structure database for inorganic compounds. Database, ASM Int Materials Park, OH:


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Pearson%27s+Crystal+Data%C2%AE%3A+crystal+structure+database+for+inorganic+compounds.&author=P+Villars&publication_year=2007&)
93. 93.

    Oliynyk AO, Adutwum LA, Rudyk BW, Pisavadia H, Lotfi S et al. 2017.  Disentangling structural confusion through machine learning: structure prediction and polymorphism of equiatomic ternary phases ABC.  J. Am. Chem. Soc. 139:17870–81

    [[Crossref]](https://doi.org/10.1021/jacs.7b08460)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/29129069) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000418204600033&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Disentangling+structural+confusion+through+machine+learning%3A+structure+prediction+and+polymorphism+of+equiatomic+ternary+phases+ABC&author=AO+Oliynyk&author=LA+Adutwum&author=BW+Rudyk&author=H+Pisavadia&author=S+Lotfi&journal=J.+Am.+Chem.+Soc.&volume=139&doi=10.1021%2Fjacs.7b08460&pages=17870-81&publication_year=2017&)
94. 94.

    Seko A, Hayashi H, Kashima H, Tanaka I 2018.  Matrix-and tensor-based recommender systems for the discovery of currently unknown inorganic compounds.  Phys. Rev. Mater. 2:013805

    [[Crossref]](https://doi.org/10.1103/PhysRevMaterials.2.013805)
    [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000423135500002&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Matrix-and+tensor-based+recommender+systems+for+the+discovery+of+currently+unknown+inorganic+compounds&author=A+Seko&author=H+Hayashi&author=H+Kashima&author=I+Tanaka&journal=Phys.+Rev.+Mater.&volume=2&doi=10.1103%2FPhysRevMaterials.2.013805&pages=013805&publication_year=2018&)
95. 95.

    Belsky A, Hellenbrandt M, Karen VL, Luksch P 2002.  New developments in the Inorganic Crystal Structure Database (ICSD): accessibility in support of materials research and design.  Acta Crystallogr. B 58:364–69

    [[Crossref]](https://doi.org/10.1107/S0108768102006948)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/12037357) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000176270700008&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=New+developments+in+the+Inorganic+Crystal+Structure+Database+%28ICSD%29%3A+accessibility+in+support+of+materials+research+and+design&author=A+Belsky&author=M+Hellenbrandt&author=VL+Karen&author=P+Luksch&journal=Acta+Crystallogr.+B&volume=58&doi=10.1107%2FS0108768102006948&pages=364-69&publication_year=2002&)
96. 96.

    Lu S, Zhou Q, Ouyang Y, Guo Y, Li Q, Wang J 2018.  Accelerated discovery of stable lead-free hybrid organic–inorganic perovskites via machine learning.  Nat. Commun. 9:3405

    [[Crossref]](https://doi.org/10.1038/s41467-018-05761-w)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Accelerated+discovery+of+stable+lead-free+hybrid+organic%E2%80%93inorganic+perovskites+via+machine+learning&author=S+Lu&author=Q+Zhou&author=Y+Ouyang&author=Y+Guo&author=Q+Li&author=J+Wang&journal=Nat.+Commun.&volume=9&doi=10.1038%2Fs41467-018-05761-w&pages=3405&publication_year=2018&)
97. 97.

    Wu S, Kondo Y, Kakimoto M, Yang B, Yamada H et al. 2019.  Machine-learning-assisted discovery of polymers with high thermal conductivity using a molecular design algorithm.  npj Comput. Mater. 5:66

    [[Crossref]](https://doi.org/10.1038/s41524-019-0203-2)

    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Machine-learning-assisted+discovery+of+polymers+with+high+thermal+conductivity+using+a+molecular+design+algorithm&author=S+Wu&author=Y+Kondo&author=M+Kakimoto&author=B+Yang&author=H+Yamada&journal=npj+Comput.+Mater.&volume=5&doi=10.1038%2Fs41524-019-0203-2&pages=66&publication_year=2019&)
98. 98.

    Otsuka S, Kuwajima I, Hosoya J, Xu Y, Yamazaki M 2011.  PoLyInfo: polymer database for polymeric materials design.  2011 International Conference on Emerging Intelligent Data and Web Technologies22–29 Piscataway, NJ: IEEE


    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=PoLyInfo%3A+polymer+database+for+polymeric+materials+design&author=S+Otsuka&author=I+Kuwajima&author=J+Hosoya&author=Y+Xu&author=M+Yamazaki&journal=2011+International+Conference+on+Emerging+Intelligent+Data+and+Web+Technologies&pages=22-29&publication_year=2011&)
99. 99.

    Ramakrishnan R, Dral PO, Rupp M, Von Lilienfeld OA 2014.  Quantum chemistry structures and properties of 134 kilo molecules.  Sci. Data 1:140022

    [[Crossref]](https://doi.org/10.1038/sdata.2014.22)
    [[Medline]](https://pubmed.ncbi.nlm.nih.gov/25977779) [[Web of Science]](https://www.webofscience.com/api/gateway?GWVersion=2&SrcApp=umwos_03&SrcAuth=WosAPI&KeyUT=WOS:000209843500015&DestLinkType=FullRecord&DestApp=WOS_CPL)
    [[Google Scholar]](http://scholar.google.com/scholar_lookup?title=Quantum+chemistry+structures+and+properties+of+134+kilo+molecules&author=R+Ramakrishnan&author=PO+Dral&author=M+Rupp&author=OA+Von+Lilienfeld&journal=Sci.+Data&volume=1&doi=10.1038%2Fsdata.2014.22&pages=140022&publication_year=2014&)

/content/journals/10.1146/annurev-matsci-090319-010954

![Loading](/images/jp/spinner.gif)

Machine Learning in Materials Discovery: Confirmed Predictions and Their Underlying Approaches

Annual Review of Materials Research 50, 49 (2020); [https://doi.org/10.1146/annurev-matsci-090319-010954](https://doi.org/10.1146/annurev-matsci-090319-010954 "undefined - opens in new window/tab")

/content/journals/10.1146/annurev-matsci-090319-010954

/content/journals/10.1146/annurev-matsci-090319-010954

![Loading](/images/jp/spinner.gif)

Data & Media loading...

### Most Read This Month

Article

* + ### [Beta-Gallium Oxide Material and Device Technologies](/content/journals/10.1146/annurev-matsci-080921-104058)

    Masataka Higashiwaki and
    Man Hoi Wong

    pp.
    175–198
    (24)
* + ### [Circular Steel for Fast Decarbonization: Thermodynamics, Kinetics, and Microstructure Behind Upcycling Scrap into High-Performance Sheet Steel](/content/journals/10.1146/annurev-matsci-080222-123648)

    Dierk Raabe,
    Matic Jovičević-Klug,
    Dirk Ponge,
    Alexander Gramlich,
    Alisson Kwiatkowski da Silva,
    A. Nicholas Grundy,
    Hauke Springer,
    Isnaldi Souza Filho and
    Yan Ma

    pp.
    247–297
    (51)
* + ### [Gallium Liquid Metal: The Devil's Elixir](/content/journals/10.1146/annurev-matsci-080819-125403)

    Shi-Yang Tang,
    Christopher Tabor,
    Kourosh Kalantar-Zadeh and
    Michael D. Dickey

    pp.
    381–408
    (28)
* + ### [Representations of Materials for Machine Learning](/content/journals/10.1146/annurev-matsci-080921-085947)

    James Damewood,
    Jessica Karaguesian,
    Jaclyn R. Lunger,
    Aik Rui Tan,
    Mingrou Xie,
    Jiayu Peng and
    Rafael Gómez-Bombarelli

    pp.
    399–426
    (28)
* + ### [Opportunities and Challenges for Machine Learning in Materials Science](/content/journals/10.1146/annurev-matsci-070218-010015)

    Dane Morgan and
    Ryan Jacobs

    pp.
    71–103
    (33)

content/journals/matsci

Journal

5

3

false

en

## Most Cited [Most Cited RSS feed](/rss/content/journals/matsci/mostcitedarticles?fmt=rss "Subscribe to most Cited RSS feed")

* + ### [SOFT LITHOGRAPHY](/content/journals/10.1146/annurev.matsci.28.1.153)

    [Younan Xia](/search?value1=Younan+Xia&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true) and
    [George M. Whitesides](/search?value1=George+M.+Whitesides&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 28
    (1998),
    pp.
    153–184
* + ### [Synthesis and Characterization of Monodisperse Nanocrystals and Close-Packed Nanocrystal Assemblies](/content/journals/10.1146/annurev.matsci.30.1.545)

    [C. B. Murray](/search?value1=C.+B.+Murray&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true),
    [C. R. Kagan](/search?value1=C.+R.+Kagan&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true) and
    [M. G. Bawendi](/search?value1=M.+G.+Bawendi&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 30
    (2000),
    pp.
    545–610
* + ### [Phase-Field Models for Microstructure Evolution](/content/journals/10.1146/annurev.matsci.32.112001.132041)

    [Long-Qing Chen](/search?value1=Long-Qing+Chen&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 32
    (2002),
    pp.
    113–140
* + ### [Wetting and Roughness](/content/journals/10.1146/annurev.matsci.38.060407.132434)

    [David Quéré](/search?value1=David+Qu%C3%A9r%C3%A9&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 38
    (2008),
    pp.
    71–99
* + ### [THE MATERIAL BONE: Structure-Mechanical Function Relations](/content/journals/10.1146/annurev.matsci.28.1.271)

    [S. Weiner](/search?value1=S.+Weiner&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true) and
    [H. D. Wagner](/search?value1=H.+D.+Wagner&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 28
    (1998),
    pp.
    271–298
* + ### [Proton-Conducting Oxides](/content/journals/10.1146/annurev.matsci.33.022802.091825)

    [K.D. Kreuer](/search?value1=K.D.+Kreuer&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 33
    (2003),
    pp.
    333–359
* + ### [High Rate Thick Film Growth](/content/journals/10.1146/annurev.ms.07.080177.001323)

    [J A Thornton](/search?value1=J+A+Thornton&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 7
    (1977),
    pp.
    239–260
* + ### [Inkjet Printing of Functional and Structural Materials: Fluid Property Requirements, Feature Stability, and Resolution](/content/journals/10.1146/annurev-matsci-070909-104502)

    [Brian Derby](/search?value1=Brian+Derby&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 40
    (2010),
    pp.
    395–414
* + ### [Mussel-Inspired Adhesives and Coatings](/content/journals/10.1146/annurev-matsci-062910-100429)

    [Bruce P. Lee](/search?value1=Bruce+P.+Lee&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true),
    [P.B. Messersmith](/search?value1=P.B.+Messersmith&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true),
    [J.N. Israelachvili](/search?value1=J.N.+Israelachvili&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true) and
    [J.H. Waite](/search?value1=J.H.+Waite&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 41
    (2011),
    pp.
    99–132
* + ### [Strongly Geometrically Frustrated Magnets](/content/journals/10.1146/annurev.ms.24.080194.002321)

    [A P Ramirez](/search?value1=A+P+Ramirez&option1=author&noRedirect=true&sortField=prism_publicationDate&sortDescending=true)

    Vol. 24
    (1994),
    pp.
    453–480
* [More](#)
  [Less](#)

---

*爬取时间: 2025-11-28 21:53:41*
