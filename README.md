# E-commerce Customer Feedback Analysis & Business Intelligence

## Project Overview

This capstone project demonstrates advanced data classification and summarization techniques using **IBM Granite 3.3-8B-Instruct** model to analyze e-commerce customer feedback. The project combines sentiment analysis, product categorization, and business intelligence generation to provide actionable insights for e-commerce businesses.

### 🎯 Project Objectives
- **Classify** customer reviews by sentiment and product issues
- **Summarize** business insights from customer feedback patterns  
- **Visualize** key metrics and trends in customer satisfaction
- **Generate** actionable recommendations for business improvement

## 🗂️ Raw Dataset

**Dataset Source**: Custom-created comprehensive e-commerce reviews dataset  
**Dataset Link**: Available in `customer_reviews_analysis.csv`

### Dataset Specifications:
- **Total Reviews**: 12 customer reviews
- **Product Categories**: 5 categories (Smartphone, Laptop, Headphones, Smartwatch, Tablet)
- **Rating Scale**: 1-5 stars
- **Date Range**: January 2024
- **Review Features**: 
  - Review ID, Product Category, Review Text
  - Customer Rating, Review Date

### Sample Data Structure:
```json
{
  "review_id": "R001",
  "product_category": "Smartphone", 
  "review_text": "The battery lasts all day and the camera quality is amazing...",
  "rating": 5,
  "date": "2024-01-15"
}
```

## 🔍 Analysis Process

### 1. **Data Classification with IBM Granite**
- **Sentiment Analysis**: Positive/Negative/Mixed classification
- **Issue Identification**: Automatic detection of product problems
- **Strength Recognition**: Identification of product advantages
- **Category Mapping**: Performance/Design/Value/Reliability analysis

### 2. **Business Summarization**
- **Executive Summary**: High-level business insights
- **Category Analysis**: Performance by product type
- **Critical Issues**: Most common customer complaints
- **Positive Highlights**: Top appreciated features
- **Actionable Recommendations**: Data-driven business advice

### 3. **Data Visualization & Analytics**
- Rating distribution analysis
- Product category performance
- Timeline trends
- Interactive dashboards
- Word frequency analysis

## 🎯 Key Insights & Findings

### Customer Sentiment Distribution
- **Positive Reviews**: 50% (6/12 reviews with 4-5 stars)
- **Mixed Reviews**: 25% (3/12 reviews with 3 stars)  
- **Negative Reviews**: 25% (3/12 reviews with 1-2 stars)

### Top Product Issues Identified
1. **Battery & Heat Problems**: Devices overheating during intensive use
2. **Display Issues**: Screen visibility problems in outdoor conditions
3. **Performance Bugs**: App crashes and slow response times
4. **Build Quality**: Durability concerns with cables and components

### Most Appreciated Features
1. **Battery Life**: Long-lasting performance for daily use
2. **Display Quality**: Excellent color reproduction and clarity
3. **Performance**: Smooth operation for intended use cases
4. **Design**: Comfortable and ergonomic product design

### Product Category Performance
- **Highest Rated**: Smartphones & Tablets (4.2/5.0 avg)
- **Most Reviewed**: Smartphones (33% of all reviews)
- **Improvement Needed**: Laptops (3.0/5.0 avg rating)

## 🤖 AI Support Explanation

### IBM Granite Model Implementation

**Model Used**: `ibm-granite/granite-3.3-8b-instruct`  
**Platform**: Replicate API via LangChain Community

#### Classification Tasks:
- **Prompt Engineering**: Multi-step classification prompts for sentiment and category analysis
- **Parameter Tuning**: Optimized `top_k=5`, `top_p=0.9`, `max_tokens=512` for classification accuracy
- **Batch Processing**: Efficient processing of multiple reviews simultaneously

#### Summarization Tasks:
- **Business Intelligence**: Structured prompts for executive-level insights
- **Strategic Analysis**: Comprehensive review patterns and recommendations
- **Parameter Optimization**: `top_k=10`, `top_p=0.95`, `max_tokens=800` for detailed summaries

#### AI Enhancement Benefits:
1. **Automated Sentiment Analysis**: Eliminates manual review classification
2. **Pattern Recognition**: Identifies recurring themes across large datasets
3. **Business Intelligence**: Converts raw feedback into strategic insights
4. **Scalability**: Process thousands of reviews efficiently
5. **Consistency**: Standardized analysis criteria across all reviews

## 📈 Business Recommendations

### Immediate Actions Required:
1. **Address Heat Issues**: Implement better thermal management in devices
2. **Improve Display Technology**: Enhanced outdoor visibility features
3. **Quality Assurance**: Strengthen testing for app compatibility and stability
4. **Build Quality Control**: Enhanced durability testing for accessories

### Strategic Improvements:
1. **Customer Feedback Loop**: Implement real-time review monitoring
2. **Product Development**: Focus on top-appreciated features in new products  
3. **Quality Metrics**: Establish KPIs based on customer feedback patterns
4. **Support Enhancement**: Proactive customer service for identified issues

## 🛠️ Technical Implementation

### Dependencies
```python
langchain_community==0.0.13
replicate==0.22.0
pandas==2.0.3
matplotlib==3.7.1
seaborn==0.12.2
plotly==5.17.0
wordcloud==1.9.2
```

### Model Parameters
- **Classification**: `top_k=5, top_p=0.9, max_tokens=512`
- **Summarization**: `top_k=10, top_p=0.95, max_tokens=800`
- **Repetition Penalty**: 1.1-1.2 for diverse outputs

## 📁 Project Structure
```
ecommerce-feedback-analysis/
├── notebook/
│   └── ecommerce_analysis.ipynb
├── data/
│   ├── customer_reviews_analysis.csv
│   └── analysis_results.json
├── visualizations/
│   └── generated plots and charts
├── README.md
└── requirements.txt
```

## 🚀 How to Run

1. **Setup Environment**:
   ```bash
   pip install -r requirements.txt
   ```

2. **Configure API**: Add your Replicate API token to Google Colab secrets as 'api_token'

3. **Run Analysis**: Execute all cells in the Jupyter notebook

4. **View Results**: Check generated CSV files and visualization outputs

## 📊 Results Summary

- **Processing Time**: ~5-10 minutes for complete analysis
- **Accuracy**: High-quality sentiment classification with detailed categorization
- **Business Value**: Actionable insights with specific improvement recommendations
- **Scalability**: Framework supports analysis of thousands of reviews

## 🔮 Future Enhancements

- **Real-time Analytics**: Live customer feedback monitoring
- **Multi-language Support**: Analysis of reviews in various languages  
- **Predictive Analytics**: Forecast customer satisfaction trends
- **Integration APIs**: Connect with major e-commerce platforms
- **Advanced Visualizations**: Interactive dashboards with drill-down capabilities

---

**Project Author**: [Your Name]  
**Course**: Student Development Initiative - Capstone Project  
**Model**: IBM Granite 3.3-8B-Instruct  
**Completion Date**: [Current Date]
