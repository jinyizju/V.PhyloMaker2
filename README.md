V.PhyloMaker2


This R package makes phylogenetic hypotheses for a user-specified list of species, by providing multiple ways of binding the species (tips) to a backbone phylogeny, as described in Qian & Jin (2016), Jin & Qian (2019, 2022).

Currently, this package includes two major components: (1) the functions, including ‘phylo.maker’, ‘bind.relative’, ‘build.nodes.1’, ‘build.nodes.2’, ‘at.node’, ‘int.node’ and ‘ext.node’; and (2) the data, including 'GBOTB.extended.TPL', ‘tips.info.TPL’, ‘nodes.info.1.TPL’ and ‘nodes.info.2.TPL’, 'GBOTB.extended.LCVP', ‘tips.info.LCVP’, ‘nodes.info.1.LCVP’ and ‘nodes.info.2.LCVP’, 'GBOTB.extended.WP', ‘tips.info.WP’, ‘nodes.info.1.WP’ and ‘nodes.info.2.WP’.

(1) The functions

The main function ‘phylo.maker’ performs the task of binding tips to a backbone phylogeny, which by default is the maga-phylogeny 'GBOTB.extended.TPL' of vascular plants embedded in the package.

The function ‘bind.relative’ performs the task of binding tips to the their species- and genus-level closest relative in the backbone phylogeny, when information is provided. ‘bind.relative’ can work alone or with ‘phylo.maker’, for a list of species, as examplified in the function help page and Jin & Qian (2019).

The functions ‘build.nodes.1’ and ‘build.nodes.2’ extract the genus- and family- level node and age information in a phylogeny in different ways. The information extracted are used by ‘phylo.maker’ and ‘bind.relative’ in binding tips to backbone phylogeny.

The functions ‘at.node’, ‘int.node’ and ‘ext.node’ bind a tip to a phylogeny, at different places. These three functions are fast in binding tip to large phylogenies.

(2) The data

The three versions of four data sets work with the functions to make phylogenetic hypotheses for a user-specified list of vascular plant species. 

1)
‘GBOTB.extended.TPL’ is a mega-tree derived from two recently published mega-trees, described in the help page, and includes 74,529 species and all families of extant vascular plants, is the largest dated phylogeny for vascular plants.

‘tips.info.TPL’ is a data frame that contains the information of all the tips, as well as as their genus and family assignments, in ‘GBOTB.extended.TPL’.

‘nodes.info.1.TPL’ and ‘nodes.info.2.TPL’ are the genus- and family-level node and age information in ‘GBOTB.extended.TPL’ extracted by ‘build.nodes.1’ and ‘build.nodes.2’, respectively.

2)
‘GBOTB.extended.LCVP’ is a mega-tree derived from two recently published mega-trees, described in the help page, and includes 73,420 species and all families of extant vascular plants, was based on the LCVP nomenclature standardization system.

‘tips.info.LCVP’ is a data frame that contains the information of all the tips, as well as as their genus and family assignments, in ‘GBOTB.extended.LCVP’.

‘nodes.info.1.LCVP’ and ‘nodes.info.2.LCVP’ are the genus- and family-level node and age information in ‘GBOTB.extended.LCVP’ extracted by ‘build.nodes.1’ and ‘build.nodes.2’, respectively.

3)
‘GBOTB.extended.WP’ is a mega-tree derived from two recently published mega-trees, described in the help page, and includes 72,570 species and all families of extant vascular plants, was based on the WP database (https://www.worldplants.de) for standardize spellings and nomenclature.

‘tips.info.WP’ is a data frame that contains the information of all the tips, as well as as their genus and family assignments, in ‘GBOTB.extended.WP’.

‘nodes.info.1.WP’ and ‘nodes.info.2.WP’ are the genus- and family-level node and age information in ‘GBOTB.extended.WP’ extracted by ‘build.nodes.1’ and ‘build.nodes.2’, respectively.

Citation:
Jin, Y., & Qian, H. (2019). V.PhyloMaker2: An updated and enlarged R package that can generate very large phylogenies for vascular plants. Plant Diversity, https://doi.org/10.1016/j.pld.2022.05.005
Jin, Y., & Qian, H. (2019). V. PhyloMaker: an R package that can generate very large phylogenies for vascular plants. Ecography, 42(8), 1353-1359.
Smith, S. A., & Brown, J. W. (2018). Constructing a broadly inclusive seed plant phylogeny. American journal of botany, 105(3), 302-314.
Zanne, A. E., Tank, D. C., Cornwell, W. K., Eastman, J. M., Smith, S. A., FitzJohn, R. G., ... & Beaulieu, J. M. (2014). Three keys to the radiation of angiosperms into freezing environments. Nature, 506(7486), 89-92.
