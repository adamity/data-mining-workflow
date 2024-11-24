# **Standard Data Mining Workflow Cheatsheet**

This cheatsheet provides a clear, actionable guide for tackling **supervised** (with labels) and **unsupervised** (no labels) learning problems. It serves beginners as a learning guide while giving experienced practitioners a reliable checklist.

> **Tip for Beginners**: Each step helps you understand **what to search online**, making it easier to find specific tutorials or tools to guide you through your data mining journey.

---

## **1. Problem Definition**

**What Are You Trying to Solve?**

- **Define Clear Goals**
  - What problem needs solving?
  - What decisions will this help make?
  - How will success be measured?
  - What resources are available?

- **Identify Problem Type**
  - **Supervised Learning**: Predict outcomes using labeled data
    - Classification: Categories (e.g., "Will customer churn?")
    - Regression: Numbers (e.g., "What will the sales be?")
  
  - **Unsupervised Learning**: Find patterns in unlabeled data
    - Clustering: Group similar items
    - Anomaly Detection: Find unusual patterns

- **Common Pitfall**: Starting without clear success metrics
- **Best Practice**: Document your goals and constraints

---

## **2. Data Collection**

**Get Quality Data!**

- **Gather Your Data**
  - Databases and files
  - APIs and web sources
  - Surveys and forms
  - Sensors and devices

- **Key Considerations**
  - **Supervised**: Ensure you have reliable labels
  - **Unsupervised**: Focus on data quality and coverage
  - Check data freshness and relevance
  - Consider privacy and legal requirements

- **Data Documentation**
  - Record data sources
  - Note collection dates
  - Document known limitations
  - Create data dictionaries

- **Common Pitfall**: Using outdated or incomplete data
- **Best Practice**: Always validate data quality early

---

## **3. Data Preprocessing**

**Clean and Prepare Your Data**

- **Basic Cleaning**
  - Handle missing values
    - Remove if few (< 5%)
    - Fill with average/common values
    - Use advanced methods if important
  - Remove duplicates
  - Fix obvious errors

- **Data Transformation**
  - **Numbers**: Scale to similar ranges
    - Standard scaling (mean=0, std=1)
    - Min-max scaling (0 to 1)
  - **Categories**: Convert to numbers
    - One-hot encoding (for distinct categories)
    - Label encoding (for ordered categories)

- **Feature Engineering**
  - Combine related features
  - Break down complex features
  - Create domain-specific features
  - Remove redundant features

- **Special Considerations**
  - **Supervised**: Handle imbalanced classes
  - **Unsupervised**: Scale features appropriately

- **Common Pitfall**: Data leakage during preprocessing
- **Best Practice**: Create reproducible preprocessing steps

---

## **4. Data Exploration (EDA)**

**Understand Your Data**

- **Basic Analysis**
  - Check data shapes and sizes
  - View summary statistics
  - Plot distributions
  - Identify patterns

- **Relationship Analysis**
  - **Supervised**: Check feature-target relationships
  - **Unsupervised**: Look for natural patterns
  - Create correlation heatmaps
  - Plot key relationships

- **Visualization Types**
  - Histograms for distributions
  - Scatter plots for relationships
  - Box plots for outliers
  - Time plots for trends

- **Common Pitfall**: Skipping visualization
- **Best Practice**: Always plot your data

---

## **5. Model Selection**

**Choose the Right Tool**

- **Supervised Learning**
  - **Classification Models**
    - Logistic Regression: Simple, interpretable
    - Random Forest: Powerful, handles nonlinearity
    - Gradient Boosting: High performance

  - **Regression Models**
    - Linear Regression: Simple, interpretable
    - Random Forest: Handles nonlinearity
    - Gradient Boosting: High performance

- **Unsupervised Learning**
  - **Clustering**
    - K-Means: Simple, fast
    - DBSCAN: Handles complex shapes
    - Hierarchical: Shows relationships

  - **Anomaly Detection**
    - Isolation Forest: Fast, effective
    - One-Class SVM: Robust
    - Statistical Methods: Simple

- **Selection Criteria**
  - Data size and type
  - Problem complexity
  - Performance needs
  - Interpretability requirements

- **Common Pitfall**: Choosing complex models unnecessarily
- **Best Practice**: Start simple, add complexity if needed

---

## **6. Model Training**

**Build Your Model**

- **Data Splitting**
  - Training set (60-70%)
  - Validation set (15-20%)
  - Test set (15-20%)

- **Training Process**
  - **Supervised**
    - Train on training data
    - Validate on validation set
    - Keep test set untouched
    - Adjust model parameters
  
  - **Unsupervised**
    - Train on entire dataset
    - Validate using metrics
    - Adjust parameters as needed

- **Best Practices**
  - Start with simple models
  - Use cross-validation
  - Track all experiments
  - Save model checkpoints

- **Common Pitfall**: Using test data too early
- **Best Practice**: Keep test set truly separate

---

## **7. Model Evaluation**

**Check Performance**

- **Supervised Metrics**
  - **Classification**
    - Accuracy: Overall correctness
    - Precision: False positive control
    - Recall: False negative control
    - F1-Score: Balance of precision/recall
  
  - **Regression**
    - MSE/RMSE: Error magnitude
    - MAE: Average error
    - R²: Explained variance

- **Unsupervised Metrics**
  - **Clustering**
    - Silhouette Score: Cluster quality
    - Within-cluster variance
  - **Anomaly Detection**
    - Precision/Recall (if labeled)
    - Domain expert validation

- **Common Pitfall**: Relying on single metric
- **Best Practice**: Use multiple relevant metrics

---

## **8. Model Refinement**

**Make It Better**

- **Improvement Strategies**
  - Tune hyperparameters
  - Feature selection/engineering
  - Try different algorithms
  - Ensemble methods

- **Common Issues**
  - **Overfitting**: Too complex
    - Simplify model
    - Add regularization
    - Get more data
  
  - **Underfitting**: Too simple
    - Add complexity
    - Engineer better features
    - Try advanced models

- **Common Pitfall**: Over-optimizing single metric
- **Best Practice**: Balance multiple objectives

---

## **9. Deployment**

**Use It in Real World**

- **Deployment Steps**
  - Save model properly
  - Set up prediction pipeline
  - Test in real conditions
  - Monitor performance

- **Key Considerations**
  - Processing speed needs
  - Resource requirements
  - Maintenance plans
  - Backup procedures

- **Common Pitfall**: Insufficient testing
- **Best Practice**: Test thoroughly before launch

---

## **10. Monitoring and Maintenance**

**Keep It Working**

- **Regular Monitoring**
  - Track performance metrics
  - Check data quality
  - Monitor system health
  - Watch for drift

- **Maintenance Tasks**
  - Update data regularly
  - Retrain periodically
  - Fix issues promptly
  - Document changes

- **Common Pitfall**: Set-and-forget approach
- **Best Practice**: Continuous monitoring

---

## **Tips for Success**

- **For Beginners**
  - Follow steps sequentially
  - Start with simple models
  - Document everything
  - Ask for help when stuck

- **For Advanced Users**
  - Use as checklist
  - Customize for needs
  - Optimize critical parts
  - Share knowledge

---

**Remember**: This workflow is flexible - adapt it to your specific needs while keeping the core steps intact. The goal is to build effective models while following best practices!
