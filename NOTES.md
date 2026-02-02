## project notes (refer to notebooks)

exploration:

- dataset heavily imbaanced, ~90% positive reviews
- short reviews are common and ambiguous

features:

- tf-idf with 20k features
- unigrams used for baseline

modeling:

- baseline logistic egression favored positive class
- class weights {0:1.6, 1:1}, improved macro f1, could be tweaked in the future
- no deep learning intentionally

## decisions

- avoid all deep learning to focus on fundementals
- prioratize interpretability vs raw high accuracy
