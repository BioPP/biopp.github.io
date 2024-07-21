---
layout: default
---

{% for post in site.posts limit:5 %}
## [{{ post.title }}]({{ post.url }})
<!-- ### _{{ post.date | date_to_long_string }}_  -->
{{ post.excerpt }} [...]({{ post.url | absolute_url }})
{% endfor -%}

### The Bio++ Project

**Bio++** is a set of C++ libraries for Bioinformatics, including sequence analysis, phylogenetics, molecular evolution and population genetics. Bio++ is Object Oriented and is designed to be both easy to use and computer efficient. Bio++ intends to help programmers to write computer expensive programs, by providing them a set of re-usable tools. 

An overview of the libraries and the underlying methods implemented is available on the [Bio++ Wiki](https://github.com/BioPP/bpp-documentation/wiki/), as well as installation instructions.

### API documentation

Detailed documentation of the classes can be found here:
* [bpp-core](https://pbil.univ-lyon1.fr/bpp-doc/bpp-core/html/)
* [bpp-seq](https://pbil.univ-lyon1.fr/bpp-doc/bpp-seq/html/)
* [bpp-phyl](https://pbil.univ-lyon1.fr/bpp-doc/bpp-phyl/html/)
* [bpp-popgen](https://pbil.univ-lyon1.fr/bpp-doc/bpp-popgen/html/)
* [bpp-seq-omics](https://pbil.univ-lyon1.fr/bpp-doc/bpp-seq-omics/html/)
* [bpp-phyl-omics](https://pbil.univ-lyon1.fr/bpp-doc/bpp-phyl-omics/html/)
<!-- * [bpp-raa](https://pbil.univ-lyon1.fr/bpp-doc/bpp-raa/html/) -->
* [bpp-qt](https://pbil.univ-lyon1.fr/bpp-doc/bpp-qt/html/)

### Projects using the Bio++ libraries

* [The Bio++ Program Suite](http://github.com/BioPP/bppsuite/) provides a set of ready-to-use programs, allowing notably to process sequences, fit a large set of models of sequence evolution, or conduct population genetic analyses.

* [TestNH](http://github.com/BioPP/testnh/) provides some tools to fit complex non-homogeneous models, but also to perform substitution mapping. 

* [Grapes](http://github.com/BioPP/grapes/) is a tool to fit models of distributions of fitness effects on polymorphism data and estimate the rate of adaptive non-synonymous substitutions.

* [PhySamp](http://jydu.github.io/physamp/) provides programs to filter sequence alignments and phylogenies based on data availability and sequence similarity.

* [CoMap](http://jydu.github.io/comap/) is a package for the analysis of molecular coevolution.

* [MafFilter](http://jydu.github.io/maffilter/) is a genome alignment processor, allowing advanced filtering, format conversion and population genomic analyses.

### Container

An apptainer recipe is available there:

* [apptainer](http://github.com/BioPP/bpp-apptainer)

as well as a debian computed image:

* [debian](https://pbil.univ-lyon1.fr/bpp-doc/images/bpp_debian.sif)
