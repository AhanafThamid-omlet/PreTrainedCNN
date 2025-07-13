# Fruit Condition Classification Using CNN (Lab 2)

This project is part of Lab 3 for our Deep Learning course.The goal is to classify fruit conditions 
(Fresh, Rotten, Formalin-mixed) across five fruit types using a pretrained CNN model.

---

# Dataset

The dataset contains images of 5 fruit types:
- Apple
- Banana
- Grape
- Mango
- Orange

Each fruit has 3 condition folders:
- Fresh
- Rotten
- Formalin-mixed

Total Classes:15 (e.g., Apple_Fresh, Banana_Rotten, etc.)

The dataset was uploaded and used on [Kaggle](https://www.kaggle.com/datasets/thecurrent/fruit-condition).

---

## Model

We used (Transfer Learning) with a (pretrained CNN model)(ResNet1) from `torchvision.models`.  
Only the final classification layer was updated to match our custom dataset (15 classes).

---

# Steps Performed

- Loaded and explored the dataset
- Visualized class distributions
- Applied data transformations (resize, normalize)
- Created a custom PyTorch `Dataset` from image paths
- Used `train_test_split` for training/validation
- Fine-tuned a pretrained ResNet18 model
- Evaluated model accuracy

---

## Results

- **Training Accuracy:** ~`0.961`
- **Validation Accuracy:** ~`0.135`
- Final model performed reasonably well given limited data.

---

## Requirements

- Python
- PyTorch
- torchvision
- matplotlib
- scikit-learn
- pandas
- Kaggle environment

---

## Notes

- Dataset was uploaded manually to Kaggle as a folder.
- GPU acceleration was used on Kaggle for training.

---

## Author

**Ahanaf_Tahmid**  
Dept. of CSE  
East West University

---

