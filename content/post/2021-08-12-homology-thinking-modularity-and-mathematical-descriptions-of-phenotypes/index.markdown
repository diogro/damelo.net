---
title: Homology thinking, modularity, and mathematical descriptions of phenotypes
author: ''
date: '2015-11-15'
slug: homology-thinking-modularity-and-mathematical-descriptions-of-phenotypes
categories: []
tags: []
subtitle: ''
summary: ''
authors: [admin]
lastmod: '2015-11-15T19:24:22-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
bibliography: [references.bib]
csl: apa-numeric-superscript
---

# Abstract

In this essay we discuss different mathematical representation of phenotypes, focusing on morphometric landmark based data. We examine the main characteristics of linear distances, Procrustes shape representations, and local shape deformations, paying special attention to how they relate do the study of variation, which is critical in an evolutionary context. By investigating what assumptions are made by each of these representations, how they relate to a homology thinking and to the study of modularity, we can develop a better understanding of the appropriate uses for each of them, and how we can use these representations to reach meaningful biological conclusions. In particular, when studying modularity, we must use representation that preserve locality, that is, local changes are represented as such. We argue that Procrustes shape variables fail to maintain this local aspect of variation, and so should not be used in applications that study local variation.

# Introduction

In this essay, I discuss different options for mathematical representation of phenotypes, focusing on morphometric landmark based data. I examine what are the main characteristics of the different representations, and how they relate to a homology thinking.

## Brief review of homology thinking

Homology thinking is a term coined by Ereshefsky<sup>1</sup> and refers to an evolutionary biology mindset that thinks in terms of what are the units of evolutionary change that make up an organism.

Following Wagner<sup>2</sup>, I define a homolog as being a part of an organism that possesses some sort of individuality in relation to development, genetic variation and function. This individuation entails evolutionary independence, so this homolog part has it’s own *quasi*-independent lineage of evolutionary change, while still being identifiable in different individuals of the same species, and among different species.

## Characters and Landmarks

The definition of morphometric characters for evolutionary biology is often based on some idea of homology, but frequently this homology is taken to mean any type of “equivalence” between structures. Ereshefsky<sup>3</sup>, for example, says:

> *“(…) two bones are considered homologous because they occupy the same relative position in their respective organisms, even though those bones may vary in shape and size.”*

The choice of homologous landmarks in morphometrics is also based in this equivalence, and indeed Zelditch et al.<sup>4</sup> argue:

> *“If discrete and recognizable structures are homologous as structures, then discrete and recognizable locations on them are arguably homologous as points.”*

This notion of homology of landmarks is also heavily based on an idea of deformation, that is, if one structure was to be deformed into the other, the homologous landmarks would map onto one another.
Under homology thinking, the choice of traits should be informed by evolutionary independence and developmental individualization.

## Individualization

The question is then how different elements in a morphological structure are expressed. Taking the example of bone formation, cells inside a same bone or set of bones tend to come from the same embryonic cells (except when they don’t, as in the mammalian mandible). In any event, different bones are sufficiently conserved and identifiable in enough lineages for it to be plausible that they are indeed individual elements with definite homology between species. The insect wing is also an example of a homologous structure that has some degree of compartmentalization and independence between different regions. Studies with *Drosophila* show a complex pattern of differential gene expression and regulation between these regions. And how do we deal with these complex structures composed of many parts? The skull is always thought as a homologous structure present in all members of *Craniata*, but is there any gain in considering it homologous as a whole? Is there enough interdependence between its component parts to warrant the title of an individualized structure? Or, given that independent variation of the component parts, that can lead to a very diverse array of shapes and forms, is it more productive to focus on each bone individually? This choice is of course to a large degree arbitrary, but it has consequences in our choice of representation, as we see below.

# Representations

Our representations of morphological structures should be tailored to capture the phenomenon we wish to study. Evolutionary change under homology thinking is interested in understanding the changes in the individual homologous parts through time.

## Linear distances

Linear distances are the oldest form of phenotype representation.
Height, cranial length, cranial width, total body length, wing span, arm length are all distances that have been used at one time or another as traits in evolutionary studies.
Indeed, the seminal work on morphological integration by Olson and Miller<sup>5</sup> makes use of these variables throughout.
However, some of these traits are composite of many different bones, and can change in a myriad of ways that are clearly non-equivalent.
For instance, wing span in birds can change with modifications in any of the many bones in the wing of even with changes in the thorax.
One way to avoid this type of ambiguity in the observed changes is to look for homologous individualized distances.
This can be done by using individual bones, and by choosing equivalent distances that describe some aspect of each bone.
This strategy is more in line with homology thinking, and was first put forward by Pearson and Davin<sup>6</sup>, who suggested the use of distances limited to single bones that could be identified in different species. Later, Cheverud<sup>7</sup> brought this notion into quantitative genetics and morphological integration. Equivalent distances are defined by first choosing landmarks at specific positions, such as the suture between three bones, or the end of a suture<sup>4</sup>; and then calculating interlandmark distances.
While this strategy for defining the distances is subject to the same criticism of subdivision outlined above, the resulting distances give a somewhat reliable measure of a particular bone, and subtle differences in definition are likely not problematic, in the sense that changes in that particular evolutionary unit will be reflected in the distance (unless change in exactly perpendicular to the measurement).
A set of distances, each confined to a particular bone (or individualized structure) is then thought to be a set of homologous traits that can be used to describe a complex structure and compared between specimens.
An example of choosing a set of distances can be found in Cheverud 1995<sup>8</sup>.
Both changes in the mean of these traits and the covariation between them brings relevant evolutionary information<sup>9,10</sup>.
The point I wish to stress here is that, while distances may not capture the full range of possible changes in a particular trait, all change in a distance can be attributed to changes in the trait.
This means locality and individuality of homologues is preserved in this representation.

## Shape variables

Recently, the use of distances for describing morphological systems has been replaced by more formal representations of shape that are also based on landmarks<sup>11,12</sup>.
The most popular method, geometric morphometrics, uses a set of landmarks measured in many specimens and attempts to remove all effects due to size, location and rotation; and what remains after this removal is called *shape*<sup>13</sup>.
The removal of these effects is done via Generalized Procrustes Analysis (GPA<sup>14</sup>), which scales, superimposes and rotates each specimen in order to minimize the distance between the homologous landmarks in each of them and a *mean shape*.
This procedure is justified since the orientation and position of the landmarks can not be relevant for any biological question on shape, and so should be removed from the landmark data.
Removal of size is a more contentious point, since size certainly has biological meaning; but arguably two structures can have the same shape and different sizes. So, if we are interested only in shape, size should be removed, and can be analyzed separately.

In the end, the representation of landmark data in GPA has many desirable mathematical properties, such as invariance to scale and a well behaved metric between shapes<sup>14,15</sup>.
Also, unlike distances, any change in landmark position will necessarily induce a change in shape.
But, also unlike distances, no effort is made to preserve locality: every shape change is dependent on every landmark. The shape is defined by every part in relation to every other, as the Procrustes superimposition minimizes distances for all landmarks in a specimen and the mean shape simultaneously<sup>16</sup>.
This aspect of the method is usually called the *pinocchio problem*, and this is resolved with the argument that there is no natural position for a given structure, and all changes are indeed in relation to the rest of the structure.
Bringing this discussion to homology thinking, this sort of interrelatedness would only be justified if the whole of the structure being analyzed, or the full set of landmarks, had the necessary individuality in evolutionary terms. So, while GPA has a number of desirable properties, it does not preserve individuality of homologues that potentially make up a complex structure.

## Local deformations

Local deformations, or local shape variables, are a relatively new method that uses landmarks and a robust mathematical framework to represent shape in a way that preserves locality<sup>17</sup>.
In this representation, landmarks are used to fit an interpolation function between them, usually a thin plate spline, which can then be deformed to match the mean shape.
The deformation transformation from each specimen to the mean shape is the mathematical object we work with, and local derivatives (the Jacobian matrix) of the transformation function for each specimen can be taken at any point of the structure.
The determinant of these derivatives are the actual variables, and they describe how much expansion or contraction happens at each point of the structure.
These have several advantages:
(1) the variables describe local changes, so homology and individuality is preserved;
(2) the number of landmarks can be high, and this will allow a precise fit for the interpolating function, but the set of traits (where the derivatives are taken) can be decided *a posteriori*, depending on sample size or the biological question;
(3) the Jacobian of the transformation is independent of the rotation and position of the landmarks, so no superimposition or rotation is necessary;
(4) scale, or size, can be analyzed as an additional variable;
(5) we keep the advantage of every landmark shift being detected as in GPA, but the changes preserve locality, as in linear distances.

Another interesting (and novel) aspect of this representation is that we are forced to make an explicit choice as to how we model the tissue between the landmarks, which are arguably the things we are actually interested in investigating.
While the choice of thin plate splines (which in practice is an infinitely thin and malleable surface) might be criticized, at least it is explicit; and other choices for the interpolating function are possible, and can be biologically informed by biomechanical models.

# Locality and variation

So, how does the different aspects of each representation relate to variation? Patterns of variational modularity<sup>18</sup> and integration<sup>5</sup> are inferred by the statistical association between the traits in a population. Traits that are functionally and developmentally associated are expected to form variational modules, and tend to vary and change in a coordinated fashion. Identification of these modules then is critically dependent on the choice of traits and on the characterization of the association between these traits. Covariation is also an important part of understanding multivariate evolution<sup>9</sup>, and so we may ask how each of the representations affect our evolutionary inquiry.

Linear distances preserve locality and have been used in many hundreds of insightful works, but lack any information on the geometry of the traits[^1] and are less sensitive to landmark shifts that are perpendicular to the distances. Also, size variation is inherently distributed along all traits, so it is difficult to separate size variation from shape variation[^2]. Discerning associations between individual structures, or groups of traits, from global associations is also difficult, since every developmental processes will superimpose themselves in the covariation between the traits<sup>22</sup>. This is a problem in all representations, but in distances it is especially difficult, because many of the developmental processes that overlap are related to growth, and size and growth variation is pulverized in all distances by the very nature of the representation. Meanwhile, GPA variables capture all changes in landmarks and separates size, but pulverize local variation to all landmarks. This leads to serious problems in capturing associations, since changes that are restricted to one bone or region (say, more cell divisions in a particular bone) will have effects on landmarks placed in totally unrelated structures.

Indeed, works on detection of modules (groups of tightly interacting traits that are relatively independent from the rest of the organism) reach radically different conclusions depending on the choice of representation.
For example, Ivanović et al. 2005<sup>23</sup> found that the correlation between functionally related traits in European newts was higher than between traits performing different functions, consistent with the hypothesis of the relation between morphological integration and function first presented by Olson and Miller<sup>5</sup>, and the relative independence expected under modularity theory<sup>18,24</sup>.
Subsequent articles from this group moved away from linear distances and began using GPA, and in Ivanović et al. 2010<sup>25</sup>, working with alpine newts, the authors found no relation between the observed pattern of covariation in the traits and function, development and hormonal sensitivity, in stark contrast to their earlier results.
Another striking example of the effects of representation comes from the Large/Small experimental cross from Jim Cheverud’s lab.
Using these populations, genetic regions affecting morphological traits can be identified (quantitative trait loci, or QTL), and in Cheverud et al. 1997<sup>26</sup>, using linear distances in the mandible, a clear modular pattern was identified, with most QTL affecting either distances in the *corpus* region of the mandible, where teeth are inserted, or distances in the *ascending ramus*, where muscles are inserted.
These regions perform different functions and originate from different embrionary tissues, so the relative independence of genetic effects is expected.
However, working with the same data using GPA, Klingenberg et al. 2001<sup>27</sup> and 2004<sup>28</sup> found no such separation, and most QTLs affected the whole mandible.
Both examples seem puzzling if we don’t understand our representations for what they are.

### What kind of changes are important?

If we are to understand these conflicting results, we must realize that individualization (evolutionary independence, homology) between the traits under consideration is a necessary property of the representation we use if we wish to identify independent variation or localized genetic effects.
If GPA does not preserve locality, how can it be expected to bring information about variational independence in a population?
Indeed, in a recent survey of the power of detection of modules, Garcia et al. 2015<sup>29</sup> found extremely low power of module detection using GPA, and similarly high power using linear distances and local deformations. Aditionaly, linear distances and local deformations recover similar sets of traits as modules in the skull, and these modules are compatible with our knowledge function and development; while partitions coming from GPA are different and hard to reconcile with these other lines of investigation.

The point here is that using GPA is implicitly assuming that the independence of the individual elements of a complex structures is not important for our analysis, and that all variation should be relative to the full set of traits. In contrast, linear distances and local deformations focus on the putative independence of the individual traits of a complex structure. If the individual elements are indeed strongly associated, this would be apparent by the covariation structure.

# Conclusion

In this essay I have attempted to discuss the implications of homology thinking for the methodological choice of how to represent a multivariate morphological phenotype. The focus on local variation, restricted to individualized homologous traits, allows us to understand some of the assumptions each of the available representations: while linear distances and local deformations set out to describe each part independently, geometric morphometrics uses the full multivariate shape as the phenotype under consideration. As such, the choice of representation is not only a methodological choice, but one that implicitly imposes a choice in how biological variation in a given structure should be represented, and what kinds of questions can be asked. While linear distances and local deformations lose shape information, relative independence and patterns of covariation can be investigated. GPA preserves all information on shape, but discards information on association between component parts. Much confusion in the recent literature is due to a failure to grasp what information is conveyed by each representation, and exaggerated focus on mathematical properties.

# Acknowledgments

Monique Simon, Guilherme Garcia, Thiago Zahn, and Fabio Machado provided helpful comments and discussion. Tiana Kohlsdorf organized the course that motivated this essay.

# References

<div id="refs" class="references csl-bib-body hanging-indent" line-spacing="2">

<div id="ref-Ereshefsky2012-wv" class="csl-entry">

1\. Ereshefsky, M. (2012). Homology thinking. *Biol. Philos.*, *27*(3), 381–400. <https://doi.org/10.1007/s10539-012-9313-7>

</div>

<div id="ref-Wagner2016-jw" class="csl-entry">

2\. Wagner, G. P. (2016). What is “homology thinking” and what is it for? *J. Exp. Zool. B Mol. Dev. Evol.*, *326*(1), 3–8. <https://doi.org/10.1002/jez.b.22656>

</div>

<div id="ref-Ereshefsky2007-mf" class="csl-entry">

3\. Ereshefsky, M. (2007). Psychological categories as homologies: Lessons from ethology. *Biol. Philos.*, *22*(5), 659–674. <https://doi.org/10.1007/s10539-007-9091-9>

</div>

<div id="ref-Zelditch2004-ih" class="csl-entry">

4\. Zelditch, M. L., Swiderski, D. L., & Sheets, H. D. (2004). *Geometric morphometrics for biologists: A primer*. Academic Press.

</div>

<div id="ref-Olson1958-qk" class="csl-entry">

5\. Olson, R., & Miller, E. (1958). *<span class="nocase">Morphological integration</span>*. University of Chicago Press.

</div>

<div id="ref-Pearson1924-sz" class="csl-entry">

6\. Pearson, K., & Davin, A. G. (1924). On the biometric constants of the human skull. *Biometrika*, *16*(3/4), 328. <https://doi.org/10.2307/2331712>

</div>

<div id="ref-Cheverud1982-op" class="csl-entry">

7\. Cheverud, J. M. (1982). <span class="nocase">Phenotypic, Genetic, and Environmental Morphological Integration in the Cranium</span>. *Evolution*, *36*(3), 499. <https://doi.org/10.2307/2408096>

</div>

<div id="ref-Cheverud1995-fd" class="csl-entry">

8\. Cheverud, J. M. (1995). <span class="nocase">Morphological Integration in the Saddle-Back Tamarin (Saguinus fuscicollis) Cranium</span>. *Am. Nat.*, *145*(1), 63–89. <https://doi.org/10.1086/285728>

</div>

<div id="ref-Lande1979-pq" class="csl-entry">

9\. Lande, R. (1979). <span class="nocase">Quantitative Genetic Analysis of Multivariate Evolution, Applied to Brain: Body Size Allometry</span>. *Evolution*, *33*(1), 402–416. <https://doi.org/10.2307/2407630>

</div>

<div id="ref-Lande1983-ez" class="csl-entry">

10\. Lande, R., & Arnold, S. J. (1983). <span class="nocase">The Measurement of Selection on Correlated Characters</span>. *Evolution*, *37*(6), 1210. <https://doi.org/10.2307/2408842>

</div>

<div id="ref-James_Rohlf1993-fk" class="csl-entry">

11\. James Rohlf, F., & Marcus, L. F. (1993). A revolution morphometrics. *Trends Ecol. Evol.*, *8*(4), 129–132. <https://doi.org/10.1016/0169-5347(93)90024-J>

</div>

<div id="ref-Corti1993-vj" class="csl-entry">

12\. Corti, M. (1993). Geometric morphometrics: An extension of the revolution. *Trends Ecol. Evol.*, *8*(8), 302–303. <https://doi.org/10.1016/0169-5347(93)90261-M>

</div>

<div id="ref-Bookstein1997-cp" class="csl-entry">

13\. Bookstein, F. L. (1997). *Morphometric tools for landmark data: Geometry and biology*. Cambridge University Press.

</div>

<div id="ref-Kendall1984-do" class="csl-entry">

14\. Kendall, D. G. (1984). Shape manifolds, procrustean metrics, and complex projective spaces. *Bull. Lond. Math. Soc.*, *16*(2), 81–121. <https://doi.org/10.1112/blms/16.2.81>

</div>

<div id="ref-Adams2013-qe" class="csl-entry">

15\. Adams, D. C., Rohlf, F. J., & Slice, D. E. (2013). A field comes of age: Geometric morphometrics in the 21st century. *Hystrix*, *24*(1), 7.

</div>

<div id="ref-Van_der_Linde2009-yx" class="csl-entry">

16\. Linde, K. van der, & Houle, D. (2009). <span class="nocase">Inferring the nature of allometry from geometric data</span>. *Evol. Biol.*, *36*(3), 311–322. <https://doi.org/10.1007/s11692-009-9061-z>

</div>

<div id="ref-Marquez2012-qe" class="csl-entry">

17\. Márquez, E. J., Cabeen, R., Woods, R. P., & Houle, D. (2012). <span class="nocase">The Measurement of Local Variation in Shape.</span> *Evol. Biol.*, *39*(3), 419–439. <https://doi.org/10.1007/s11692-012-9159-6>

</div>

<div id="ref-Wagner2007-cx" class="csl-entry">

18\. Wagner, G. P., Pavlicev, M., & Cheverud, J. M. (2007). <span class="nocase">The road to modularity</span>. *Nat. Rev. Genet.*, *8*(12), 921–931. <https://doi.org/10.1038/nrg2267>

</div>

<div id="ref-Lele1991-lk" class="csl-entry">

19\. Lele, S., & Richtsmeier, J. T. (1991). Euclidean distance matrix analysis: A coordinate-free approach for comparing biological shapes using landmark data. *Am. J. Phys. Anthropol.*, *86*(3), 415–427. <https://doi.org/10.1002/ajpa.1330860307>

</div>

<div id="ref-Mosimann1970-dz" class="csl-entry">

20\. Mosimann, J. E. (1970). <span class="nocase">Size Allometry: Size and Shape Variables with Characterizations of the Lognormal and Generalized Gamma Distributions</span>. *J. Am. Stat. Assoc.*, *65(330)*(930-945), 930–945. <https://doi.org/10.1080/01621459.1970.10481136>

</div>

<div id="ref-Sakamoto2012-jv" class="csl-entry">

21\. Sakamoto, M., & Ruta, M. (2012). Convergence and divergence in the evolution of cat skulls: Temporal and spatial patterns of morphological diversity. *PLoS One*, *7*(7), e39752. <https://doi.org/10.1371/journal.pone.0039752>

</div>

<div id="ref-Hallgrimsson2009-kq" class="csl-entry">

22\. Hallgrı́msson, B., Jamniczky, H., Young, N. M., Rolian, C., Parsons, T. E., Boughner, J. C., & Marcucio, R. S. (2009). <span class="nocase">Deciphering the Palimpsest: Studying the Relationship Between Morphological Integration and Phenotypic Covariation</span>. *Evol. Biol.*, *36*(4), 355–376. <https://doi.org/10.1007/s11692-009-9076-5>

</div>

<div id="ref-Ivanovic2005" class="csl-entry">

23\. Ivanović, A., Kalezić, M., & Aleksić, I. (2005). Morphological integration of cranium and postcranial skeleton during ontogeny of facultative paedomorphic european newts (triturus vulgaris and t. alpestris). *Amphib-Reptil.*, *26*(4), 485–495. <https://doi.org/10.1163/156853805774806223>

</div>

<div id="ref-Wagner1996-vm" class="csl-entry">

24\. Wagner, G. P. G. P. (1996). Homologues, natural kinds and the evolution of modularity. *Integr. Comp. Biol.*, *36*(1), 36–43. <https://doi.org/10.1093/icb/36.1.36>

</div>

<div id="ref-Ivanovic2010-of" class="csl-entry">

25\. Ivanović, A., & Kalezić, M. L. (2010). Testing the hypothesis of morphological integration on a skull of a vertebrate with a biphasic life cycle: A case study of the alpine newt. *J. Exp. Zool. B Mol. Dev. Evol.*, *314*(7), 527–538. <https://doi.org/10.1002/jez.b.21358>

</div>

<div id="ref-Cheverud1997-rw" class="csl-entry">

26\. Cheverud, J. M., Routman, E. J., & Irschick, D. J. (1997). Pleiotropic effects of individual gene loci on mandibular morphology. *Evolution*, *51*(6), 2006. <https://doi.org/10.2307/2411021>

</div>

<div id="ref-Klingenberg2001-cu" class="csl-entry">

27\. Klingenberg, C. P., Leamy, L. J., Routman, E. J., & Cheverud, J. M. (2001). Genetic architecture of mandible shape in mice: Effects of quantitative trait loci analyzed by geometric morphometrics. *Genetics*, *157*(2), 785–802.

</div>

<div id="ref-Klingenberg2004-xu" class="csl-entry">

28\. Klingenberg, C. P., Leamy, L. J., & Cheverud, J. M. (2004). Integration and modularity of quantitative trait locus effects on geometric shape in the mouse mandible. *Genetics*, *166*(4), 1909–1921. <https://doi.org/10.1534/genetics.166.4.1909>

</div>

<div id="ref-Garcia2015-ys" class="csl-entry">

29\. Garcia, G., Oliveira, F. B. de, & Marroig, G. (2015). *Modularity and morphometrics: Error rates in hypothesis testing*. <https://doi.org/10.1101/030874>

</div>

</div>

[^1]: Unless a large number of triangulating distances is used, as in Euclidean distance matrix analysis<sup>19</sup>, and this has its own set of problems relating to sample size requirements.

[^2]: From an evolutionary standpoint, this might not be such a serious problem, since natural selection and drift are oblivious to what we separate as size and shape. Also, see Mosimann 1970<sup>20</sup> for a way to separate shape and size using distances. This method is used in Sakamoto and Ruta 2012<sup>21</sup>.
