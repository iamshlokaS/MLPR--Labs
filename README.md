# Machine Learning and Pattern Recognition  
## Lab 5 
### Shloka Srivastava (ID: U20240131)

---

## Aim

The aim of this lab is to:

- Detect faces in images  
- Extract simple color features from faces  
- Group faces using KMeans clustering  
- Classify a new face using a template image  
- Visualize the clustering results  

---

## Method

### 1. Face Detection

- Haar Cascade classifier was used.
- Faces were detected in:
  - A group faculty image
  - A template image
- Rectangles were drawn around detected faces.

---

### 2. Feature Extraction

For each detected face:

- The face region was cropped.
- The image was converted from BGR to HSV format.
- Mean **Hue** and **Saturation** values were calculated.
- Each face was represented as a 2D point  

---

### 3. KMeans Clustering

- KMeans algorithm was applied with **k = 2**.
- Faces were divided into two clusters.
- Cluster centers (centroids) were calculated.
- Results were plotted in 2D space.

---

### 4. Template Face Classification

- A template face image was processed the same way.
- Hue and Saturation values were calculated.
- The template was assigned to the nearest cluster.
- The result was shown in the feature plot.

---

## Results

### 1. Face Detection on Group Image

30 faces were detected successfully.

![detected_faces](https://github.com/user-attachments/assets/4510c9b6-92f0-474b-b960-4c530adfc207)

---

### 2. Face Clustering (Hue vs Saturation)

Each face was plotted as a point in 2D space.
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/93519d0d-11bd-4327-9713-1160680e81ee" />



---

### 3. KMeans Clustering with Centroids

Faces were grouped into two clusters and centroids were shown.
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/a31f9a83-4ba3-454d-8f41-85ec01603dfc" />


---

### 4. Template Face in Feature Space

Template face was plotted with other faces.

<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/d5356ba5-a4c7-4ae4-8c5a-0980bb5678f8" />


---

### 5. Final Classification Result

Template face was assigned to the nearest cluster.

<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/5935583f-11a6-4495-b398-4fa30d9e1117" />

---

## Key Observations

- Haar Cascade detected faces correctly.
- Hue and Saturation gave a simple 2D representation of faces.
- KMeans successfully grouped faces into two color-based clusters.
- The template face was classified based on similarity to cluster centers.
- 2D plots clearly showed cluster separation.

---

## Conclusion

In this lab:

- Face detection was done using classical computer vision.
- Simple color features (Hue and Saturation) were used.
- KMeans grouped faces based on color similarity.
- A new face was classified using cluster distance.

This experiment shows how basic computer vision and machine learning techniques can be combined for simple face grouping and classification.
