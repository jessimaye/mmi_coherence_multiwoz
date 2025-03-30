# MMI 24/25: Evaluating Coherence in Task-Oriented Dialogues Using Large Language Models – A Re-Annotation of the MultiWOZ dataset

## Model Runs
This folder contains the jupyter-notebooks needed to connect with the llama-models for reannotating the MultiWOZ-dataset. "annotation_llama" uses the server from the University of Regensburg, "annotation_api" uses the API from the "Gesellschaft für wissenschaftliche Datenverarbeitung Göttingen" (GWDG). To run these notebooks you`ll also need "data.json" from the MultiWOZ-dataset 2.3 (source below). The dialogue-texts from this dataset are extracted in the notebook. After running the respective models, the results are saved as a list and txt.-file. 

"actions_annotation_api" is used to determine a coherence value for the dialogue actions annotation by Prof. Dr. Bernd Luwdig. The LLM is implemented via the API from the GWDG.  

Source for the original MultiWOZ-dataset: https://github.com/budzianowski/multiwoz

Source for the MultwiWOZ-dataset 2.3 used in this project: https://github.com/lexmen318/MultiWOZ-coref

## Data

The zip-file "Annotation_Coherence" containts the newly annotated MultiWOZ dialogues, including the id of the dialogue, thex text, a coherence score, an explanation for the score and the assistance functions, performed by the wizard. The annotation is available as a csv-, txt- and json-file.

## Data Processing
This folder contains the "regex-extraction" jupyter notebook for extracting the desired data from the LLM-output with regular expressions. The results are saved as dataframes. 
