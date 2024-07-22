## Biomarker-KG: Visualizing Biomarker Discovery


### Abstract

WIP 


### Biological Entities Included in Biomarker-KG
| Entity      | Description        |     Nodes |     Edges |                                      Relations|
|:----------|:-------------------|----------:|----------:|------------------------------------------------------------------------------------:|
| Anatomy   | nodes from UBERON  |       8 |     115 | "determined using sample from"                                                      |
| Compound  | nodes from PUBCHEM |      49 |      49 | "indicated by above normal level of", "indicated by below normal level of (Compound)" |
| Condidion | nodes from DOID    |     403 |  182914 | "diagnostic for", "indicates risk of developing", "prognostic for"                      |
| Role      | nodes from OBCI    |       4 |  135536 | "has best classification"                                                           |
| Variant   | nodes from DBSNP   |  133709 |  133710 | "indicated by presence of"                                                          |

### Using BKG

#### 1. Creating a subnetwork
##### 1.1 One-term Search
![Input Form]

Generating a subnetwork with BKG requires the input of a starting node. In the dropdown boxes on the left, you can select the node type you would like to look up, and whether you would like to search by id or label. Then you will need to enter the id or label underneath.

##### 1.2 Navigating the results
![Enrichment Result](https://s3.amazonaws.com/maayan-kg/enrichr-kg/assets/060624/enrichment_result.png)
Upon clicking submit, the user is redirected to the results page which should look like the image above. Nodes are colored based on their type. The results can be displayed as a bar chart showing the top enrichred terms ordered by p-value. The icons on the upper right corner enable users to: (1) display the legend; (2) refresh, re-orient, or clear the graph; (3) display the edge labels; (4) download the graph as an image (JPG, PNG, or SVG); (5) share a permanent link; and (6) enter full screen mode.

![Hover Node](https://s3.amazonaws.com/maayan-kg/enrichr-kg/assets/060624/hover.png)
Hovering over the nodes and edges invokes a text box on the top left containing the metadata of the node or edge. The has buttons to: (1) delete a node from the subnetwork; (2) go to the node's page to view its immediate neighbors; and (3) close the box.

## Please acknowledge Enrichr-KG in your publications by citing the following reference:

[Evangelista JE, Xie Z, Marino GB, Nguyen N, Clarke DJB, Ma'ayan A. Enrichr-KG: bridging enrichment analysis across multiple libraries. Nucleic Acids Res. 2023 May 11:gkad393. doi: 10.1093/nar/gkad393. PMID: 37166973.](https://academic.oup.com/nar/article/51/W1/W168/7160192)