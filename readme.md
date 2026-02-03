# Learning Probability Density Functions using Non-Linear Transformation and MLE

This project demonstrates how a probability density function (PDF) can be learned from air quality data using a roll-number-based non-linear transformation and Maximum Likelihood Estimation (MLE).

## Dataset
- India Air Quality Dataset
- Feature used: NO₂ (Nitrogen Dioxide) concentration
- Source: Kaggle  
  https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data

## Objective
- Apply a personalized non-linear transformation to NO₂ data
- Model the transformed data using a Gaussian-type PDF
- Estimate PDF parameters using Maximum Likelihood Estimation
- Visualize and analyze the learned distribution

## Methodology
- Load dataset with robust encoding handling
- Automatically detect the NO₂ column
- Remove missing values
- Apply roll-number-based non-linear transformation  
  z = x + a_r sin(b_r x)
- Analyze statistics before and after transformation
- Assume a Gaussian-type probability density function
- Estimate parameters using MLE

## Results
- Mean (μ): 25.8074
- Lambda (λ): 0.00146
- Normalization constant (c): 0.02156

## Visualizations
- Histogram of original NO₂ values
- Histogram of transformed variable
- Learned PDF overlaid on transformed data

## Conclusion
The experiment shows that non-linear transformations combined with Maximum Likelihood Estimation can effectively model real-world air quality data. The roll-number-based approach ensures personalization while maintaining statistical validity.
