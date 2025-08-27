# Semantic_segmentation-Cam_Vid

This project was developed as part of a university course on Deep Learning.  
It focuses on semantic segmentation using the CamVid dataset, which contains annotated driving scenes.  

- **Dataset**: CamVid urban driving scenes with 11 semantic classes.  
  - Training set: 367 samples  
  - Validation set: 101 samples  
  - Test set: 233 samples  

- **Model**: Implemented an **encoder–decoder CNN architecture** (similar to U-Net) for pixel-wise segmentation.  

- **Loss Functions**:  
  - **Dice Loss**, particularly effective for imbalanced data.  
  - A **hybrid loss** combining Dice Loss and Sparse Categorical Cross-Entropy to balance pixel accuracy and region-level overlap.  

- **Training**:  
  - Applied preprocessing and data augmentation.  
  - Conducted a **systematic hyperparameter search** to optimize model architecture and training settings.  
  - Training monitored with **EarlyStopping** 

- **Evaluation**:  
  - Metrics include **Intersection over Union (IoU)** per class, **mean IoU**, and **pixel accuracy**.  
  - Final evaluation conducted on the dedicated test set.  

- **Goal**: Achieve accurate semantic segmentation of driving scenes, distinguishing categories such as road, buildings, vehicles, pedestrians, vegetation, and sky.  


