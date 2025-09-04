# CI/CD Build Analysis and Interactive Dashboard

## Project Overview
This project focuses on analyzing and visualizing CI/CD pipeline metrics to improve build success rates, optimize resource usage, and support better DevOps decision-making. It uses a simulated dataset of CI/CD build metrics but can easily be extended to real pipeline data from Jenkins, GitHub Actions, or GitLab CI.

The outcome is an interactive dashboard that helps developers and DevOps teams monitor builds, compare deployment strategies, and identify inefficiencies in the pipeline.

## Problem Statement
CI/CD pipelines generate large amounts of data including build times, code complexity, test coverage, and resource utilization. Without proper analysis, it becomes difficult to identify failure patterns, track performance, and optimize deployment strategies. This project solves the problem by providing an interactive tool to explore metrics and gain insights.

## Features
- Simulated dataset with CI/CD metrics such as build time, test coverage, code complexity, CPU usage, memory usage, and deployment strategies.  
- Interactive dashboard with filters for author and deployment strategy.  
- Visualizations include:  
  - Build time vs predicted success probability (scatter plot)  
  - Average success rate by deployment strategy (bar chart)  
  - Distribution of files changed per build (histogram)  
  - CPU vs memory usage (scatter plot)  
  - Code complexity vs test coverage (scatter plot)  
  - Resource efficiency distribution (histogram)  

## Dataset
The project currently uses a synthetic dataset of 200 records, generated within the notebook. It can be replaced with real CI/CD data. Expected columns include:  

`author`, `deploy_strategy`, `files_changed`, `lines_changed`, `num_tests`, `test_coverage`, `code_complexity`, `build_time_minutes`, `cpu_usage`, `memory_usage_gb`, `build_success`, `predicted_success_prob`, `resource_efficiency`.

## How to Use
1. Open `CI_CD_Analysis.ipynb` to review simulated data and analysis.  
2. Open `CI_CD_Dashboard.ipynb` to explore the interactive dashboard.  
3. Run all cells in Jupyter Notebook or Google Colab.  
4. Use dropdown filters to explore builds by author or deployment strategy.  

## Technologies Used
- Python  
- Pandas and NumPy  
- Plotly Express for interactive visualizations  
- ipywidgets for interactive filters  
- Jupyter Notebook / Google Colab  

## Outcomes
- Dashboard for monitoring CI/CD build performance.  
- Ability to detect inefficiencies in build processes.  
- Insights into trade-offs between code complexity, test coverage, and build success.  
- Framework ready for integration with real-world CI/CD logs.  

## Future Enhancements
- Connect with Jenkins, GitHub Actions, or GitLab CI logs.  
- Use machine learning to predict build failures.  
- Export results as automated PDF or HTML reports.  
- Deploy the dashboard as a standalone web application.  
