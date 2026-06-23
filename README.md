# 📊 Google Play Store Category Performance Dashboard

> A Data Analytics and Visualization project that analyzes top-performing Google Play Store app categories based on ratings, reviews, and installs using Python and Matplotlib.

---

# 📑 Table of Contents

- <a href="#project-title">Project Title</a>
- <a href="#brief-summary">Brief One Line Summary</a>
- <a href="#overview">Overview</a>
- <a href="#problem-statement">Problem Statement</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools-and-technologies">Tools and Technologies</a>
- <a href="#methods">Methods</a>
- <a href="#key-insights">Key Insights</a>
- <a href="#dashboard-model-output">Dashboard / Output</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#how-to-run-this-project">How to Run this Project?</a>
- <a href="#results-conclusion">Results & Conclusion</a>
- <a href="#future-work">Future Work</a>
- <a href="#author-contact">Author & Contact</a>

---

<h2 id="project-title">📌 Project Title</h2>

# Google Play Store Category Performance Dashboard

---

<h2 id="brief-summary">📝 Brief One Line Summary</h2>

A Python-based analytical dashboard that evaluates top-performing Google Play Store categories using average ratings, total reviews, and installation metrics through grouped bar chart visualizations.

---

<h2 id="overview">📖 Overview</h2>

The Google Play Store contains millions of applications across multiple categories. Understanding which categories perform best based on user engagement metrics can help developers, businesses, and analysts make better strategic decisions.

This project analyzes Google Play Store application data, applies business-driven filters, aggregates category-level performance metrics, and visualizes the top-performing categories using a dual-axis grouped bar chart.

The dashboard focuses on categories with high ratings, larger application sizes, and recent updates, providing meaningful insights into app market performance.

---

<h2 id="problem-statement">⚠️ Problem Statement</h2>

Analyzing app category performance manually is difficult due to the large volume of available applications and diverse performance indicators.

This project aims to:

- Identify top-performing app categories
- Compare category-wise ratings and reviews
- Analyze installation trends
- Filter high-quality applications
- Visualize category performance effectively
- Support data-driven decision making

---

<h2 id="dataset">📂 Dataset</h2>

The project uses a Google Play Store dataset containing application details.

### Dataset Features

- App Name
- Category
- Rating
- Reviews
- Size
- Installs
- Last Updated

### Data Cleaning Performed

- Rating conversion to numeric values
- Review count cleaning
- Install count cleaning
- App size standardization
- Date conversion
- Missing value handling

---

<h2 id="tools-and-technologies">🛠️ Tools and Technologies</h2>

## Programming Language

- Python

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Datetime
- ZoneInfo

## Development Environment

- Jupyter Notebook
- VS Code

---

<h2 id="methods">⚙️ Methods</h2>

## 1. Data Preprocessing

The following preprocessing steps were applied:

### Rating Cleaning

```text
Converted ratings into numeric format
```

### Reviews Cleaning

```text
Converted review counts into numeric values
```

### Installs Cleaning

```text
10,000+ → 10000
1,000,000+ → 1000000
```

### App Size Standardization

- MB values retained
- KB values converted into MB
- Invalid values removed

### Date Processing

```text
Last Updated → Datetime Format
```

---

## 2. Business Rule Filtering

Applications were filtered using:

### Rating Filter

```text
Rating ≥ 4.0
```

### App Size Filter

```text
Size ≥ 10 MB
```

### Date Filter

```text
Updated in January
```

Only applications satisfying all conditions were included in the final analysis.

---

## 3. Category Aggregation

For each category, the following metrics were calculated:

- Average Rating
- Total Reviews
- Total Installs

---

## 4. Top Category Selection

The top 10 categories were selected based on:

```text
Total Installs
```

This helps focus the analysis on the most popular app categories.

---

## 5. Time-Based Dashboard Visibility

The dashboard includes a time-control mechanism using IST timezone.

### Dashboard Availability

```text
3:00 PM IST → 5:00 PM IST
```

This demonstrates how dashboards can be restricted to specific business hours.

---

## 6. Visualization

A grouped dual-axis bar chart was created using Matplotlib.

### Left Axis

```text
Average Rating
```

### Right Axis

```text
Total Reviews
```

### X-Axis

```text
Top 10 App Categories
```

---

<h2 id="key-insights">📊 Key Insights</h2>

- High-install categories generally maintain strong user ratings.
- User reviews provide a strong indication of category popularity.
- Categories with larger applications often sustain high engagement.
- Recently updated applications tend to perform better.
- Aggregated category analysis simplifies market trend identification.

---

<h2 id="dashboard-model-output">📈 Dashboard / Output</h2>

## Dashboard Workflow

```text
Google Play Store Dataset
          ↓
Data Cleaning
          ↓
Business Rule Filtering
          ↓
Category Aggregation
          ↓
Top 10 Category Selection
          ↓
Dual-Axis Grouped Bar Chart
```

---

## 📊 Visualization Generated

### Grouped Bar Chart

Displays:

- Average Rating per Category
- Total Reviews per Category
- Top 10 Categories by Installs

### Dual Axis Representation

| Axis | Metric |
|--------|---------|
| Left Axis | Average Rating |
| Right Axis | Total Reviews |

### Category Ranking

Categories are ranked according to:

```text
Total Installs
```

---

<h2 id="project-structure">📁 Project Structure</h2>

```bash
Google_Play_Store_Category_Performance/

│
├── task5.ipynb
├── google_play_store_dataset.csv
├── README.md
└── outputs/
```

---

<h2 id="how-to-run-this-project">🚀 How to Run this Project?</h2>

## Clone Repository

```bash
git clone https://github.com/yashrajmohanty03-ai/google-play-store-category-performance.git

cd google-play-store-category-performance
```

## Install Dependencies

```bash
pip install pandas numpy matplotlib
```

## Run Notebook

```bash
jupyter notebook task5.ipynb
```

## Execute All Cells

Run all notebook cells sequentially to:

- Load dataset
- Clean app data
- Apply filters
- Aggregate category metrics
- Select top-performing categories
- Generate grouped bar chart

---

<h2 id="results-conclusion">📈 Results & Conclusion</h2>

## Results

The dashboard successfully:

- Cleaned and transformed Google Play Store data
- Filtered high-quality applications
- Aggregated category-level metrics
- Identified top 10 categories by installs
- Compared ratings and reviews visually
- Generated an insightful dual-axis dashboard

---

## Conclusion

This project demonstrates how data analytics and visualization techniques can be used to evaluate category-level performance in the Google Play Store ecosystem. By combining ratings, reviews, and installation metrics, the dashboard provides actionable insights that can help developers and businesses understand market trends and user engagement patterns.

---

<h2 id="future-work">🔮 Future Work</h2>

Future enhancements include:

- Interactive Plotly dashboards
- Streamlit deployment
- Real-time Google Play Store data integration
- Predictive category performance analysis
- Business intelligence reporting
- Advanced user sentiment analysis
- Power BI dashboard integration

---

<h2 id="author-contact">👨‍💻 Author & Contact</h2>

## Yashraj Mohanty

### Areas of Interest

- Data Analytics
- Data Visualization
- Business Intelligence
- Machine Learning

### Contact

- GitHub: https://github.com/yashrajmohanty03-ai
- LinkedIn: https:// linkedin.com/in/yashraj-mohanty
- Email: yashrajmohanty3@gmail.com

---

<p align="center">
⭐ If you found this project useful, consider giving it a star on GitHub!
</p>