# multilingual-abstrct

This repository contains a medical corpus of argument mining [AbstRCT corpus](https://gitlab.com/tomaye/abstrct) (a dataset of clinical abstracts annotated for argument mining in English), and generation of the dataset in Spanish, French and Italian by translation and projection using word alignment tools, such as Awesome align.

# Data

The dataset consists of abstracts of 5 disease types for argument component detection and argument relation classification:

- `neoplasm`: 350 train, 100 dev and 50 test abstracts
- `glaucoma_test`: 100 abstracts
- `mixed_test`: 100 abstracts (20 on glaucoma, 20 on neoplasm, 20 on diabetes, 20 on hypertension, 20 on hepatitis) 

The structure of the repository:

Inside `EN` folder:
  - argument_components/
  - argument_relations/

Inside `ES/FR/IT` folder: 
  
  - `argument_components/$MT_$projection/`

      - `automatic_projections` - post-processed projections 
      - `manual_revision` - manually corrected projections
      - `postprocessed` - merged English and Spanish train and dev sets
      
  - `argument_relations` (Only English and Spanish (deepl))
