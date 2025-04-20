# 🚢 Sea-Vessels Detection: Development Branch

Welcome to the development branch of our project!  
Here, you'll find all the core code and resources used in dataset creation, annotation, and training of our neural networks (YOLOv8 and YOLO-E based models).

---

## 📌 Project Pipeline

Our work is structured in the following key stages:

1. **Collecting Existing Datasets**  
   We sourced initial data from well-known and reputable platforms:  
   - [Kaggle](https://www.kaggle.com/)  
   - [Roboflow](https://roboflow.com/)
   - etc.

2. **Data Review & Evaluation**  
   We previewed and analyzed the collected datasets to assess their quality, relevance, and applicability to our task. Based on this, we decided which datasets to retain.

3. **Building a Custom Dataset**  
   Since our use case is quite unique and the available open-source data was insufficient or inconsistent, we created a custom dataset using publicly available resources and knowledge bases on watercraft.

4. **Annotation of Ship Data**  
   After building our dataset, we utilized advanced annotation tools like [CVAT.ai](https://cvat.ai/) to precisely label ships within the images.

5. **Model Training**  
   Using the annotated dataset, we trained our YOLO-based models.  
   Our first trained YOLOv8 model represents the **alpha version** of this project.

---

## 🚧 Current Status

- ✅ First alpha version trained using YOLOv8
- 🔜 Planned improvements:
  - Enhancing annotation quality
  - Training improved model versions
  - Expanding the dataset with new examples

---

## 📂 What's in This Branch

- Source code for data processing and training
- Dataset management scripts
- Trained YOLOv8 alpha model
- Configuration files and annotation formats
- Future model improvement experiments

---

Stay tuned — this branch is where all active development happens.  
For stable and tested releases, refer to the `main` branch.
