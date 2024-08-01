## Biomarker-KG: Visualizing Biomarker Discovery

### Entities within BKG
#### ID's for each entity type come from sources as follows: 
- [Glygen](https://glygen.org/biomarker-search/) for biomarkers 
- [PubChem](https://pubchem.ncbi.nlm.nih.gov/) for compounds 
- [dbSNP](https://www.ncbi.nlm.nih.gov/snp/) for variants 
- [DOID Ontology](https://www.ebi.ac.uk/ols4/ontologies/doid) for conditions 
- [UBERON](https://www.ebi.ac.uk/ols4/ontologies/uberon) for anatomy
- OBCI for roles

### Using BKG Explorer

#### 1. Creating a subnetwork
##### 1.1 One-Term Search
![One-Term Search](https://s3.amazonaws.com/maayan-kg/biomarker-kg/assets/one-term.png)

Generating a subnetwork with one-term search requires the input of a starting entity. In the dropdown boxes on the panel on the left titled "Start with", you can first select the entity type you would like to look up and whether you would like to search by id or label. Then you will need to enter the ID or label underneath. 

For example, if we want to search up a biomarker and we know the label, we can select "Biomarker" in the first dropdown box and select "label". Then we can enter the biomarker's label and the following subnetwork will be generated automatically!
 of rs881844 in ERBB2" is related to 

##### 1.2 Refining the search by relation
![Refine by Dropdown](https://s3.amazonaws.com/maayan-kg/biomarker-kg/assets/refine_by_dropdown.png)

With BKG Explorer, you can refine your results in various ways. In the picture above, we want to see the specific samples from which the biomarker was measure from. To do this, we can use the "Select Relation" dropdown to select the relation "determined_using_sample_from". The generated graph indicates the different samples the biomarker was taken from by the yellow nodes: tissue and blood.

##### 1.3 Refining the search by target node type


You can also limit the subnetwork's results by specifying a target node type! You can do this by clicking on one of the node icons at the top of the page. In the picture above, we clicked the "Condition" icon to generate the subnetwork with edges specifically from biomarkers to conditions. This subnetwork shows the various conditions that the biomarker either indicates risk for or is prognostic for, depending on the edge label.

##### 1.4 Changing the subnetwork display

With BKG Explorer, there are various ways to change the way the subnetwork is displayed and saved! You can use the slider bar above the network view to increase or decrease the maximum amount of relations you wish to display for each relation type. For example, sliding the bar to "5" will display at most 5 edges of each relation. On the right, the full-screen icon will display the subnetwork in full-screen. The first two mini icons next to the full-screen icon represent viewing the subnetwork as 1. a graph or 2. a table. The next two icons represent two ways to save the subnetwork: 1. as tsv files separated by nodes and edges or 2. as a png. The last group of icons refer to ways to change the network view: 1. enabling tooltips which each node's metadata as you hover over them; 2. switching the graph layout to be i. force-directed, ii. hierarchichal, and iii. geometric; 3. showing edge labels; and 4. showing a legend to see the different node types each color represents.

##### 1.5 Two-term Search
![Two-Term Search](https://s3.amazonaws.com/maayan-kg/biomarker-kg/assets/two-term.png)

Generate a more complex subnetwork with BKG Explorer's Two-term Search! First enter a starting node similar to the one-term search and then toggle "end node". This will produce another node field for you to enter the ending node. In the picture above, we wanted to generate a subnetwork of all the nodes and edges that connect two conditions "lung carcinoma" and "neurilemmona". The generated subnetwork gave us a biomarker which indicates risk of both of them! Alternatively when looking up the end node, you can omit the id or label from the lookup tab and you would see all nodes of type Condition that are closest related to the starting node.

There are a few use cases on the "Use Case" page that provide some applications of the two-term search in a clinical context!