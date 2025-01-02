**Full writeup/explanation**: [LINK](https://www.kaggle.com/code/smitbajaj/set-a-framework-to-evaluate-edge-setters) | 
**Frontend tool:**  [LINK](https://www.kaggle.com/code/smitbajaj/set-a-framework-to-evaluate-edge-setters) |
**Frontend repo:**  [LINK](https://github.com/VSandwar74/NFL) 

## Exposing Coverage Tells in the Presnap

This repo presents a Transformer-based model that achieves 89% accuracy in pre-snap man/zone coverage prediction, peaking at 93% one second after the snap. The accompanying frontend tool (linked above) acts as an interactive football field, allowing users to experiment with defensive alignments and observe how adjustments impact coverage probabilities. We also include movement pattern maps that highlights which defenders most frequently telegraph their team's coverage and how they do it. 

For any modeling/visualization questions, reach out to @smitbajaj [LINK](https://github.com/smitbajaj) & frontend questions, reach out to @VSandwar74 LINK](https://github.com/VSandwar74).

### Instructions/Documentation
The notebooks in `notebooks-bdb-2025` are in a sequential order as follows:
 1. `cleaning_functions.ipynb` standardizes the raw tracking data & prepares for tensor input.
 2. `creating_dataloaders.ipynb` applies cleaning functions & places all frames into week-to-week tensors.
 3. `training.ipynb` defines Transformer class & iterates through leave-one-out training.
 4.   `predictions.ipynb` loads in the best model for each week & runs out of sample predictions for each frame.
 5. `id_tell_plays.ipynb` filters through significant probability swings (Part IV of write-up) & IDs "giveaway" players.
 6. `charting_paths.ipynb` charts non-motion & motion giveaway paths (needs to be cleaned)

