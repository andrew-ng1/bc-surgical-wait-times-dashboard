# BC Surgical Wait-Time Dashboard

This project analyzes 12 years (2009–2021) of surgical wait time data in British Columbia and presents it through an **interactive dashboard** built with a **Plotly Dash web app**, providing insights for healthcare administrators and the public.  
The dashboard highlights waitlist sizes, surgery completions, and wait time distributions across procedures, hospitals, and health authorities.

This project was originally developed as part of the UBC Master of Data Science program (team project, 2021).

Originally deployed on Heroku (deployment discontinued); see screenshots below for the live dashboard interface.

---

## Project Highlights
- **EDA**: Analyzed trends in surgical wait-times, revealing backlog growth and regional disparities across BC.
- **Dashboard**: Interactive web application built with **Plotly Dash** for exploring wait-times by year, region, and surgery type.
- **Deployment**: Originally deployed on Heroku for public access (can also run locally with Python).
- **Impact**: Provides actionable insights to aid the BC government and health administrators in **resource allocation and planning**.

---

## Tech Stack
- **Languages**: Python (pandas, numpy)
- **Visualization**: Dash
- **Deployment**: Heroku
- **Other Tools**: Jupyter Notebook (EDA), Git/GitHub

---

## Dataset
- Source: BC Surgical Wait-Time Data (public dataset)
- Format: CSV (12 years of data, cleaned and structured)
- Included: A **csv file** (`data.csv`) for demonstration

---

## About this Dashboard

The app uses six radio buttons to delivery corresponding information for the six health authorities. We designed five tabs to display of our data and variables. The first tab provides summary information about the dashboard in overall. The second tab provides the information about the number of waiting and completed cases summary and for different procedure groups. The third tab provides the information about the number of waiting and completed cases summary and for different hospitals. The fourth tab provides summary information on average wait times, and for both 50% and 90% of cases completed by procedure. The fifth tab provides summary information on average wait times, and for both 50% and 90% of cases completed by hospitals. Data is displayed for five tabs can be visualized over selected health authorities.

<img src="docs/sketch/surgical-dashboard.gif" width="700"/>

---

## Key Insights (from EDA)

- EDA revealed significant backlog growth post-2020, regional disparities across health authorities, and long-tail delays where 90th percentile wait times far exceeded medians.
- Backlogs grew steadily: the number of patients waiting for surgery increased over time, especially after 2020 (COVID period).
- Completed cases dipped during 2020–2021, showing the pandemic backlog effect.
- Wait times (90th percentile) are much higher than the median, highlighting extreme delays for some patients.
- Differences across health authorities: some regions consistently had longer waits and bigger backlogs than others.

---

### Installation instructions

In order to install this dashboard app and run in your local computer, please follow these steps:

1.-Install dependencies

    pip install -r requirements.txt


2.-Clone the repo to your local computer, navigate to a location you desired using `cd path` and clone our project from this Github repository using command:


    git clone repo_path


3.-In the terminal, navigate to the project directory using `cd path` and run the following command, please note if there is any package dependency missing please install using `pip install package_name`:


    python app.py
    
    
4.-Copy the link `localhost` from the terminal and enter to your web browser to view the dash app.