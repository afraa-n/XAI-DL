## Explainable Deep Learning Analysis: Understanding CNN Decision Patterns in MNIST Digit Classification
**Name: Afraa Noureen**

### 1. Hypothesis
Null Hypothesis (H₀): There is no significant difference in the sensitivity patterns of digits 6 and 8 when analyzed through occlusion-based saliency mapping.

Alternative Hypothesis (H₁): The sensitivity patterns of digits 6 and 8 differ, with digit 8 demonstrating increased sensitivity in specific regions.

### 2. Approach Overview
This assignment uses occlusion-based saliency mapping to analyze how a Convolutional Neural Network (CNN) processes and distinguishes between digits 6 and 8 in the MNIST dataset. The approach involves:

a. Training a custom CNN architecture on MNIST  
b. Implementing occlusion saliency mapping  
c. Analyzing regional sensitivity patterns  
d. Statistical comparison of sensitivity distributions  

### 3. Results

#### Regional Sensitivity Overview: 
For Digit 6, the middle region shows the highest sensitivity at 0.7985. This means that the model depends a lot on this central part of the digit to make its classification. The bottom region has a lower sensitivity of 0.2181, while the top region is even less important, with a sensitivity of 0.1997.
On the other hand, Digit 8 has a different pattern. The middle region has a much higher sensitivity of 8.3545, indicating that this part is really important for the model’s recognition of this digit. The top region has a sensitivity of 1.9607, and the bottom region sits at 1.3313. While both of these areas matter, they are not nearly as critical as the middle region.


#### Statistical Significance:
The t-statistic is -17.8344, and the p-value is 0.0000. This tells us there is a significant difference in regional sensitivities between digits 6 and 8. Since the p-value is much smaller than 0.05, we can reject the null hypothesis. This supports our alternative hypothesis that the sensitivity patterns for digits 6 and 8 are different.


#### Visualizations

The visualizations created during this analysis provide important information:

Original Images: The original images of digits 6 and 8 from the MNIST dataset are clear, showing the features that the model needs to identify.  

Saliency Maps: The saliency maps point out which parts of the digits are most important for the model’s classification:   
- For Digit 6, the saliency map highlights the middle region, which matches the higher sensitivity we found earlier.  
- For Digit 8, the saliency map also focuses on the middle region, but with even more emphasis, which goes along with the high sensitivity value of 8.3545.

Regional Comparison: The bar chart compares the sensitivities of the different regions between the two digits, making it easy to see how the model views each digit.

![image](https://github.com/user-attachments/assets/cb716664-327a-436d-9c41-e033aa2fc133)


### 4. Conclusions

Statistical Significance: The analysis shows that there is a significant difference in sensitivity patterns between digits 6 and 8, allowing us to reject the null hypothesis.  
Pattern Analysis: The results indicate that while both digits have high sensitivity in the middle region, Digit 8 relies even more on this area for classification, as reflected in its much higher sensitivity values.  
Key Findings: This assignment shows that the CNN model processes digits 6 and 8 differently, which aligns with the structural differences between the two digits.
The focus on the middle region for both digits suggests that this area contains key features needed for their classification, with Digit 8 needing extra attention in this region.
