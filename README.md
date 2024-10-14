
# ZindiChallengeModel
## Goal: In Progress
### Description
___
In Sub-Saharan Africa, crop diseases and pests lead to an annual 40% loss in yield, affecting both food security and the economy. Agriculture employs over 60% of the population and contributes 23% of the region’s GDP.

Climate change and limited access to technology are worsening the spread of diseases such as **tomato leaf curl virus** and **pepper blight**, impacting crucial crops. This challenge aims to create machine learning models that can:
- **Accurately detect diseases** in images of **corn**, **pepper**, and **tomato** crops.
- **Generalize** to new diseases not in the training data.
- **Run efficiently** on entry-level smartphones used by subsistence farmers.

These models will help ensure timely disease detection, boost agricultural productivity, and promote food security for millions.

![zindi image](zindi.png)  
> [View the competition](https://zindi.africa/competitions/ghana-crop-disease-detection-challenge)

### Evaluation
___
Submissions will be evaluated using **Mean Average Precision (mAP) @ IoU threshold 0.5**. Your submission file format should look like this:

```plaintext
Image id class confidence ymin xmin ymax xmax
ID_2TZLLT80 Rot 0.5 130 12 340 300
```
- **Image_Id**: Unique ID for each image.
- **Class**: Disease classification (e.g., Rot, Blight).
- **Confidence Score**: Confidence level of the prediction, used to rank bounding boxes.

### Explainability
___
All submitted solutions must include explainability components. Participants are required to integrate techniques such as **Grad-CAM**, **LIME**, or **SHAP** to provide clear visual explanations of model predictions, ensuring transparency and fostering trust in AI solutions. This is a requirement for winning in this challenge.

### Resource Restrictions
___
Your solutions must function in a resource-limited setting (i.e., run on low-resource smartphones). The following restrictions apply:
- **T4 GPU**: Maximum 9 hours of training, maximum 3 hours of inference.
- Model frameworks must be suitable for edge devices (e.g., **ONNX**, **TensorFlow Lite**).

### Timeline
___
**Start Date**: 4 October 2024, 8:00 AM GMT  
**End Date**: 15 December 2024, 11:59 PM GMT  
Final submissions must be made by the deadline. Timeline adjustments may be announced if necessary.
