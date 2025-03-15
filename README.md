# MSLR-Web10K Hilbert Analyzer

A comprehensive toolkit for analyzing the MSLR-Web10K (Microsoft Learning to Rank) dataset using Hilbert space visualizations and advanced analytics. This repository provides deep insights into query characteristics, document relationships, and ranking patterns to help researchers understand and improve learning-to-rank algorithms.

## Table of Contents

- [Overview](#overview)
- [Analysis Methods](#analysis-methods)
- [Visualization Outputs](#visualization-outputs)
- [Integration with Ranking Systems](#integration-with-ranking-systems)

## Overview

The MSLR-Web10K dataset is a popular benchmark for learning to rank algorithms. It contains feature vectors extracted from query-document pairs along with relevance judgments on a scale from 0 (irrelevant) to 4 (perfectly relevant). This toolset employs Hilbert curve visualizations and advanced analytical techniques to explore various aspects of the dataset, revealing insights that might be missed by traditional analysis methods.

This analysis provides a deeper understanding of the dataset's characteristics, helping researchers develop more effective ranking algorithms and better evaluation methodologies.

## Analysis Methods

This toolkit provides a comprehensive set of analysis methods to explore different aspects of the MSLR dataset:

### 1. Relevance Distribution Patterns Analysis
Maps documents to a 2D Hilbert space and identifies well-structured vs. ambiguous relevance patterns. Critical for understanding how clearly defined the relevance judgments are, which affects learnability by ranking algorithms.

### 2. Query Difficulty Assessment
Evaluates query difficulty based on relevance distribution and feature characteristics. This helps identify challenging queries where ranking algorithms typically struggle, enabling focused improvement efforts.

### 3. Feature-Relevance Relationships
Identifies regions in feature space where similar documents have consistent or inconsistent relevance judgments. Crucial for finding potential annotation errors or subtle relevance factors not captured by current features.

### 4. Query Type Classification
Categorizes queries as navigational, informational, or transactional based on relevance patterns. Important for developing specialized ranking strategies for different query intents.

### 5. Cross-Fold Consistency Analysis
Measures consistency of relevance judgments across dataset folds. Essential for reliable evaluation, as inconsistent judgments can lead to misleading performance assessments.

### 6. Dataset Quality Assessment
Provides a comprehensive evaluation of dataset quality by aggregating metrics from multiple analyses. Vital for understanding dataset limitations before training models.

### 7. Ranking Algorithm Error Analysis
Identifies common patterns in ranking errors to reveal systematic weaknesses in algorithms. Helps focus development efforts on the most problematic cases.

### 8. Advanced Feature Importance Analysis
Uses permutation methods to assess feature importance and detects redundant features. Critical for feature selection and understanding which signals truly drive relevance.

### 9. Document Clustering Analysis
Clusters documents within queries to find natural groupings and compares with relevance judgments. Reveals whether relevance aligns with natural document groupings.

### 10. Query Similarity and Grouping Analysis
Groups similar queries based on feature distributions and relevance patterns. Enables transfer learning and the development of query-type-specific ranking strategies.

### 11. Fairness and Bias Analysis
Examines potential biases in relevance judgments across different dimensions. Essential for ensuring ranking systems don't perpetuate or amplify dataset biases.

### 12. SERP Diversity Analysis
Evaluates the diversity of top-ranked documents for each query. Critical for understanding whether results cover diverse aspects of queries rather than being redundant.

### 13. User Behavior Simulation
Models different user behaviors to predict how users would interact with ranked results. Bridges the gap between offline metrics and real-world effectiveness.

### 14. Robustness Analysis
Tests stability of relevance judgments by introducing small perturbations to document features. Identifies potentially unstable judgments that could negatively impact learning.

## Visualization Outputs

The analysis creates various directories with visualizations and summary files:

1. **relevance_patterns/**: Visualizations of well-structured vs. ambiguous queries
2. **query_difficulty/**: Visualizations of query difficulty analysis
3. **feature_relevance/**: Visualizations of feature-relevance relationships
4. **query_types/**: Visualizations of query type distributions
5. **cross_fold/**: Visualizations of cross-fold consistency
6. **data_quality/**: Visualizations of dataset quality assessment
7. **ranking_errors/**: Visualizations of ranking algorithm errors
8. **feature_importance/**: Visualizations of feature importance
9. **document_clustering/**: Visualizations of document clusters
10. **query_similarity/**: Visualizations of query relationships
11. **bias_analysis/**: Visualizations of potential biases
12. **user_behavior/**: Visualizations of user behavior simulations
13. **fairness/**: Visualizations of fairness and diversity analysis

## Integration with Ranking Systems

The insights from this analysis can be used to:

1. **Improve ranking algorithms**: By understanding error patterns and feature importance
2. **Develop query-specific strategies**: Using query type and difficulty classifications
3. **Identify dataset issues**: Through quality, bias, and consistency analysis
4. **Evaluate ranking systems**: With user behavior simulations and diversity metrics
5. **Enhance training strategies**: By using robustness and feature redundancy information

## Citation

If you use this code in your research, please cite:

```
@misc{mslr-hilbert-analyzer,
  author = {Setu Chokshi},
  title = {MSLR-Web10K Hilbert Analyzer},
  year = {2025},
  publisher = {GitHub},
  url = {https://github.com/setuc/mslr-hilbert-analyzer}
}
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.
