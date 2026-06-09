# 📘 Assignment: Building Interactive Web Dashboards

## 🎯 Objective

Build a web-based dashboard that visualizes and presents data interactively. You'll combine Python backend skills with frontend visualization to create a dynamic interface that brings data to life.

## 📝 Tasks

### 🛠️ Design and Build a Data Visualization Dashboard

#### Description
Create a dashboard that loads data, processes it, and displays interactive visualizations. Students should choose a dataset of interest and design the dashboard layout and visual components.

#### Requirements
Completed program should:

- Load and parse data from a CSV or external API
- Create multiple visualizations (charts, graphs, tables)
- Display at least 3 different data perspectives
- Update or filter data based on user input
- Be responsive and visually organized

#### Example
```python
import streamlit as st
import pandas as pd
import plotly.express as px

df = pd.read_csv('data.csv')

st.title("Sales Dashboard")
st.write("Overview of Q2 Performance")

col1, col2 = st.columns(2)
with col1:
    st.metric("Total Sales", "$45,000")
with col2:
    st.metric("Growth", "+12%")

fig = px.bar(df, x='region', y='sales')
st.plotly_chart(fig)
```

### 🛠️ Add Interactivity and User Controls

#### Description
Implement filters, dropdowns, and controls that let users customize what data they see without writing code.

#### Requirements
Completed program should:

- Include at least 2 filter options (date range, category, region, etc.)
- Update visualizations in real-time when filters change
- Show summary statistics that reflect filtered data
- Handle edge cases (empty filters, missing data)

### 🛠️ Enhance with Advanced Features (Stretch Goal)

#### Description
Extend the dashboard with performance optimization, caching, or multi-page navigation.

#### Requirements
Completed program should:

- Implement data caching or lazy loading for performance
- Add multiple dashboard pages/tabs for different metrics
- (Optional) Deploy to a public platform (Streamlit Cloud, Heroku, etc.)
- Include documentation explaining data sources and how to use the dashboard
