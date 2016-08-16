# bdathlon-multicell
SBOL as it currently stands can support multicellular modeling. Each cell can be encapuslated in a `ModuleDefinition`, and all cells and any small molecules within a larger `ModuleDefinition`. To indicate that this data is about a multicellular construct, annotations should be included which point to an ontology for multicellular information.

Such a repository can be found [here.](http://webprotege.stanford.edu/#Edit:projectId=323e1baf-78b7-4694-88bb-79e8a933b269) This is only a very bare-bones example, and it would be built up to include diverse host cells, culture information, and other data. However, this will allow for the standardization of terms like specific cell lineages, host media preparations, transformation procedures, and other synthetic method data. 

Because it does not require any additional functionality on behalf of SBOL, extant tools can be used to annotate the modules with SBML mathematical models to describe production and interactions, and to simulate the multicellular behavior using any simulator which supports SBML. For example, [iBioSim](http://www.async.ece.utah.edu/ibiosim) can tag the model with SBML mathematical models or simply convert the entire construct to SBML. It can then perform several simulation types and visualize the results.

## Next Steps
To create a robust ontology, a wide survey of extant systems biology publications and procedures would need to be performed. This would allow the identification of common cell species, culture media, growth conditions, and preparation procedures. Right now, only the top-level categories are present and require further work to be useful

## There's no code!
You're right! This problem has largely been solved by the work of developing a [convertor between SBOL to SBML](http://co.mbine.org/events/COMBINE_2014/agenda?q=system/files/roehner_model_generation.pdf) and the concept of annotating SBOL documents with information that has not yet been integrated fully into the standard or is only supported by a subset of tools. Thus, only the ontology allowing for the standardization of multicellular concepts was necessary to address this problem!
