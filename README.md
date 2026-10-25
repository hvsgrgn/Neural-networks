# Neural Networks

A collection of machine learning and data analysis projects in Jupyter notebooks. They range from classic data exploration with pandas and scikit-learn to neural networks in PyTorch, including fine-tuning a pretrained CNN for image classification and object detection.

## Projects

| Notebook | Task | Methods |
|---|---|---|
| [AcademicPrediction](AcademicPrediction.ipynb) | Predict students' final grades from personal and school data ([UCI Student Performance](http://archive.ics.uci.edu/ml/datasets/Student+Performance)), as a **regression** and as a **multi-class classification** problem | PyTorch MLP, handling missing data, train/val/test split, confusion matrix |
| [WineQualityPrediction](WineQualityPrediction.ipynb) | Separate "typical" wines from "unusual" ones (where tasters disagreed strongly), using their chemical properties | PyTorch MLP binary classifier, missing-value imputation, early stopping, feature importance analysis |
| [PictureClassification](PictureClassification.ipynb) | Tell photos of things that can fly (planes, birds) from everything else | Transfer learning: fine-tuning **MobileNetV2** pretrained on ImageNet, data augmentation, true/false positive/negative analysis |
| [WheresWaldo](WheresWaldo.ipynb) | Find Waldo in large "Where's Waldo?" puzzle images | Synthetic training data generation, fine-tuned MobileNetV2 binary classifier, sliding-window detection with bounding boxes |
| [PollutionAnalyzer](PollutionAnalyzer.ipynb) | Analyze nitrogen and phosphorus water pollution and how it relates to the state of the sewage system | pandas data cleaning, matplotlib/seaborn plots, interactive **Folium** maps, correlation heatmap, decision tree classifier, linear regression |

## Tech stack

- **Python** with Jupyter / Google Colab
- **PyTorch** and **torchvision** for neural networks, MobileNetV2 and data augmentation
- **scikit-learn** for decision trees, linear regression and metrics
- **pandas**, **NumPy** and **SciPy** for working with the data
- **matplotlib**, **seaborn** and **Folium** for plots and maps
- **OpenCV**, **Pillow** and **scikit-image** for image processing

## Running the notebooks

The easiest way is **Google Colab**. Open a notebook on GitHub, then upload it to [colab.research.google.com](https://colab.research.google.com/). The image notebooks (PictureClassification, WheresWaldo) need a GPU, which you can turn on under **Runtime → Change runtime type**.

To run them locally:

```
pip install torch torchvision scikit-learn pandas numpy scipy matplotlib seaborn folium opencv-python pillow scikit-image jupyter
jupyter notebook
```

The course notebooks download their datasets and test scripts from the university server, which may no longer be available. PollutionAnalyzer expects a `data.csv` file next to the notebook, and that file isn't included in this repo.

## About

These were university assignments and exams from an artificial neural networks course and a data analysis course (2025). The task descriptions and some comments inside the notebooks are in Hungarian.
