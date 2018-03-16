# CCO Examples in VRA Core 4.0

## Aims

This project aims to make available all Cataloging Cultural Objects examples ( http://cco.vrafoundation.org/index.php/toolkit/index_of_examples/ ) in the data standard of VRA Core ( http://www.core.vraweb.org/index.html ).

## Problems

Wherever possible, this project aims to include all information from the repositories in addition to what is given in the Examples. This has led to some issues of uncertainty.

### Exhibition

Although both Date and Location posses a type="exhibition", the link between certain dates and locations cannot be made more specific. To counter this, a general exhibition information has been inserted into the Description field, and the names of the exhibitions usually along with the dates have been inserted into the location refid subelement, with type="other".

### Provenance

As there is currently no separate set for provenance, this information has been included in the Description. Please see former owners for other observations.

### Subject

The subject types in the CCO examples, like in Example 11, have not been incorporated because of VRA Core's own types for subjects. 

### Textref

Fortunately, many institutions give the visitor ample information on textual sources concerning the cultural object in their care. However, these have most often proven to be too much information for this project, and as such, their incorporation was more often than not neglected.

### Depicted persons, patrons and former owners

According to the VRA Core Element Description, the agents listed in the AgentSet have "contributed to the design, creation, production, manufacture, or alteration of the work or image." It may be argued that patrons belong to this defintion.

#### Depicted persons

Identifiable depicted persons have been made part of the subjectSet, in line with the CCO Examples and the general logic of the VRA Core. However, this doesn't allow for a precise definition of their role with or without a controlled vocabulary like the marcrelator, as their listing in the agentSet would. It also omits any dates associated with them.

#### Former owners

Although the locationSet allows for the type of formerOwner, this is optimized for repositories that have or had a known location. In case of persons, however, the exact location of the object in their property isn't neccessarily available, and there is no place to attach dates associated with the person(s).

# CCO-Samples

To "clean up" the data files you can use ant (with build.xml for "data_old" or build_new.xml for "data_new") with the default target or run the xslt-files in the following order:

1. cleanup-basic.xsl
1. cleanup-types.xsl
1. cleanup-source.xsl
1. cleanup-sort.xsl
1. cleanup-dates.xsl
1. cleanup-sets.xsl
1. cleanup-empty.xsl
1. cleanup-basic.xsl
