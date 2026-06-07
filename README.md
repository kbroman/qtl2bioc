### R/qtl2bioc

[![R-CMD-check](https://github.com/rqtl/qtl2bioc/workflows/R-CMD-check/badge.svg)](https://github.com/rqtl/qtl2bioc/actions)
[![r-universe badge](https://rqtl.r-universe.dev/qtl2bioc/badges/version)](https://rqtl.r-universe.dev/qtl2bioc)

[Karl Broman](https://kbroman.org)

[R/qtl2bioc](https://github.com/rqtl/qtl2bioc) is part of [R/qtl2](https://kbroman.org/qtl2).
It uses
[Bioconductor](https://bioconductor.org) facilities to obtain
the set of mouse genes in a region. While the functions within
[R/qtl2bioc](https://github.com/rqtl/qtl2bioc) could logically be
included within [qtl2](https://github.com/rqtl/qtl2), we've kept
it separate in order to reduce package dependencies for those not
interested in making use of the
[Bioconductor](https://bioconductor.org) features.

---

### Installation

To install [R/qtl2bioc](https://github.com/rqtl/qtl2bioc), first install
the Bioconductor packages
[GenomicRanges](https://bioconductor.org/packages/release/bioc/html/GenomicRanges.html) and
[AnnotationHub](https://bioconductor.org/packages/release/bioc/html/AnnotationHub.html):

```r
install.packages("BiocManager")
BiocManager::install(c("GenomicRanges", "AnnotationHub"))
```

Next, install R/qtl2bioc from
[r-universe](https://rqtl.r-universe.dev/qtl2bioc):

```r
install.packages("qtl2bioc", repos=c("https://rqtl.r-universe.dev",
                                     "https://cloud.r-project.org"))
```

Alternatively, install the [remotes package](https://remotes.r-lib.org)
and use `remotes::install_github()` to install R/qtl2bioc from its
[Github repository](https://github.com/rqtl/qtl2bioc).

```r
install.packages("remotes")
library(remotes)
install_github("rqtl/qtl2bioc")
```

---

### Usage

The [R/qtl2bioc](https://github.com/rqtl/qtl2bioc) package contains two
key functions, `grab_ensembl()`, for downloading the
[Ensembl](https://ensembl.org) gene annotations, and
`create_ensembl_query_func()`, for creating a query function to
grab gene records for a given region.

---

#### License

[Licensed](LICENSE.md) under [GPL-3](https://www.r-project.org/Licenses/GPL-3).
