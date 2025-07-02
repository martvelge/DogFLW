# DogFLW 🐶
`Dog Facial Landmarks in the Wild (DogFLW)` dataset contains 4335 images of dogs' faces in various environments and conditions, annotated with 46 facial landmarks and a bounding box on the dog’s face.

You can download the `DogFLW` dataset from [Kaggle](https://www.kaggle.com/datasets/georgemartvel/dogflw).

Some examples from the dataset:
![](/doges.png)

## Scheme

The 46 dog facial landmarks were specifically chosen for their relationship with underlying musculature and relevance to dog-specific facial Action Units ([DogFACS](https://animalfacs.com/dogfacs_new)). You can find more details in the [dataset paper](https://arxiv.org/abs/2305.04232).

## Format

```
train/test/
│
├── images/
│ ├── name_1.png
│ │ ...
│ └── name_n.png
└── labels/ 
  ├── name_1.json
  │ ├── "labels" # (48,2)
  │ └── "bounding_boxes" # (x_1, y_1, x_2, y_2)
  │ ...
  └── name_n.json 
```

## References

If you use the `DogFLW`, please cite the [paper](https://www.nature.com/articles/s41598-025-07040-3):

```
@article{martvel2025dog,
  title     = {Dog facial landmarks detection and its applications for facial analysis},
  author    = {George Martvel and Anna Zamansky and Giulia Pedretti and Chiara Canori and Ilan Shimshoni and Annika Bremhorst},
  journal   = {Scientific Reports},
  year      = {2025},
  volume    = {15},
  number    = {1},
  pages     = {21886},
  doi       = {10.1038/s41598-025-07040-3},
  url       = {https://doi.org/10.1038/s41598-025-07040-3},
  issn      = {2045-2322}
}
```

## Contributions and Acknowledgements

The dataset was created by [Tech4Animals Lab](https://www.tech4animals.org) and supported by the [Data Science Research Center](https://dsrc.haifa.ac.il/?playlist=1d7a133&video=c6e22b5) at the University of Haifa. We thank Ephantus Kanyugi for his contribution to data annotation and management and Yaron Yossef for his technical support.

## License
This dataset is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License.
https://creativecommons.org/licenses/by-nc/4.0/
