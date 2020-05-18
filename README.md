# MouseFM: In-silico methods for finemapping of genetic regions in inbred mice
[![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?hashtags=asd&url=https://www.biorxiv.org/content/...)

&nbsp;+ [Introduction](#Introduction)\
&nbsp;+ [Installation](#Installation)\
&nbsp;+ [Usage](#Usage)\
&nbsp;&nbsp;&nbsp;&nbsp;|-- [Accepted query terms](#Accepted-query-terms)\
&nbsp;&nbsp;&nbsp;&nbsp;|-- [Optional parameters](#Optional-parameters)\
&nbsp;&nbsp;&nbsp;&nbsp;|-- [Meta information](#Meta-information)\
&nbsp;+ [Try out online](#Try-out-online)\
&nbsp;+ [Authors](#Authors)\
&nbsp;+ [Citation](#Citation)\
&nbsp;+ [License](#License)


## Introduction
This **R** package provides methods for **genetic finemapping** in **inbred mice** by taking advantage of their **very high homozygosity rate** (>95%). 

For one ore more chromosomal regions (**GRCm38**), method `finemap` extracts homozygous SNPs for which the allele differs between two sets of strains (e.g. case vs controls) and outputs respective causal SNP/gene candidates.

Method `prio` allows to **select additional strains** which best resolve a specified genetic region, e.g. QTL found by a crossing experiment of two inbred mouse strains. The selected additional strains can then be used to refine the region in further crossing experiments.


## Available inbred strains
| No | Strain             | No | Strain    | No | Strain      |
|----|--------------------|----|-----------|----|-------------|
| 1  | 129P2/OlaHsd       | 14 | C57BR/cdJ | 26 | MOLF/EiJ    |
| 2  | 129S1/SvImJ        | 15 | C57L/J    | 27 | NOD/ShiLtJ  |
| 3  | 129S5/SvEvBrd      | 16 | C58/J     | 28 | NZB/B1NJ    |
| 4  | A/J                | 17 | CAST/EiJ  | 29 | NZO/HlLtJ   |
| 5  | AKR/J              | 18 | CBA/J     | 30 | NZW/LacJ    |
| 6  | BALB/cJ            | 19 | DBA/1J    | 31 | PWK/PhJ     |
| 7  | BTBR T + Itpr3tf/J | 20 | DBA/2J    | 32 | RF/J        |
| 8  | BUB/BnJ            | 21 | FVB/NJ    | 33 | SEA/GnJ     |
| 9  | C3H/HeH            | 22 | I/LnJ     | 34 | SPRET/EiJ   |
| 10 | C3H/HeJ            | 23 | KK/HiJ    | 35 | ST/bJ       |
| 11 | C57BL/10J          | 24 | LEWES/EiJ | 36 | WSB/EiJ     |
| 12 | C57BL/6            | 25 | LP/J      | 37 | ZALENDE/EiJ |
| 13 | C57BL/6NJ          |    |           |    |             |

## Installation
```R
devtools::install_github('matmu/MouseFM', build_vignettes = TRUE)
```

**Please note**: A valid internet connection (HTTP port: 80) is required in order to install and use the package.

## Help pages
```R
browseVignettes("MouseFM")
help(package="MouseFM")
```

## Loading package
```{r}
library(MouseFM)
```

## Try out online
If you want to try out the R package online, there is an example **Google Colaboratory** project at

https://colab.research.google.com/drive/1i1sjQHCjaw2wYzVBnXQ9iaghnk-jSU95#scrollTo=5Hi6sCe7SPFb

To run the project, make a private copy or open the project in playground mode and sign in to Google. 


## Authors
Matthias Munz [![](https://img.shields.io/twitter/follow/_MatthiasMunz?label=Follow&style=social)](https://img.shields.io/twitter/follow/_MatthiasMunz?label=Follow&style=social)\
University of Lübeck, Germany


## Citation
Please cite the following article when using our tool:


## License
GNU General Public License v3.0
