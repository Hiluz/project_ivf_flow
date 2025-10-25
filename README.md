# {{crew_name}} Crew

Welcome to the {{crew_name}} Crew project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <3.14 installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```

### Customizing

**Add your `OPENAI_API_KEY` into the `.env` file**

- Modify `src/project_ivf_flow/config/agents.yaml` to define your agents
- Modify `src/project_ivf_flow/config/tasks.yaml` to define your tasks
- Modify `src/project_ivf_flow/crew.py` to add your own logic, tools and specific args
- Modify `src/project_ivf_flow/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your flow and begin execution, run this from the root folder of your project:

```bash
crewai run
```

This command initializes the project_ivf_flow Flow as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The project_ivf_flow Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the {{crew_name}} Crew or crewAI.

- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.


##תיאור:
פרויקט זה עוסק בשאלה: 
כיצד משתנה שיעור ההצלחה  בטיפולי הפריה חוץ גופית כתלות בגיל המטופלת ובסוג מחזור הטיפול (טרי לעומת מוקפא) לאורך השנים?
│
לינק ל
https://docs.crewai.com/en/guides/flows/first-flow 


הגדרת הצוותים והסוכנים:
 צוות 1: Data Preprocessing & Analysis                      │
├─────────────────────────────────────────────────────────────┤
│ 1.1 Data Cleaner → Clean Data                              │
│ 1.2 Data Validator → Validation Report                     │
└────────────┬────────────────────────────────────────────────┘
             │
             ↓
┌─────────────────────────────────────────────────────────────┐
│ צוות 2: Exploratory Data Analysis                          │
├─────────────────────────────────────────────────────────────┤
│ 2.1 Trend Analyst → Trends Report                          │
│ 2.2 Age Impact Analyst → Age Analysis                      │
│ 2.3 Cycle Comparative → Comparison Report                  │
└────────────┬────────────────────────────────────────────────┘
             │
             ↓
┌─────────────────────────────────────────────────────────────┐
│ צוות 3: Statistical Modeling                               │
├─────────────────────────────────────────────────────────────┤
│ 3.1 Time Series Forecaster → Forecast Model                │
│ 3.2 Regression Model Agent → Model Coefficients            │
│ 3.3 Scenario Generator → Scenario Matrix                   │
└────────────┬────────────────────────────────────────────────┘
             │
             ↓
┌─────────────────────────────────────────────────────────────┐
│ צוות 4: Insights & Interpretation                          │
├─────────────────────────────────────────────────────────────┤
│ 4.1 Clinical Insights → Clinical Recommendations           │
│ 4.2 Key Findings → Summary Points                          │
└────────────┬────────────────────────────────────────────────┘
             │
             ↓
┌─────────────────────────────────────────────────────────────┐
│ צוות 5: Visualization & Reporting                          │
├─────────────────────────────────────────────────────────────┤
│ 5.1 Report Generator → Final Report                        │
│ 5.2 Visualization Spec → Chart Specifications              │
│ 5.3 Stakeholder Summary → Tailored Summaries               │
└─────────────────────────────────────────────────────────────┘

שאלות ניתוח מרכזיות
📌 Key Analysis Questions
כל סוכן צריך להשיב על שאלות ספציפיות:
שאלות סוכן 2.2 (Age Impact):

איזה גיל בעל שיעור הצלחה הגבוה ביותר?
כמה קטן שיעור ההצלחה לכל שנת גיל?
מהי הנקודת תמורה (cutoff age)?

שאלות סוכן 2.3 (Cycle Comparison):

מתי Frozen cycles עלו על Fresh cycles?
מה ההבדל באחוזים?
מהן האפקטיביות היחסית?

שאלות סוכן 3.1 (Forecasting):

מה ההצלחה הצפויה ב-2025 לכל קטגוריה?
מה טווח הביטחון 95%?
מהו הקצב השיפור השנתי הצפוי?

שאלות סוכן 4.1 (Clinical):

מה הבחירה האופטימלית עבור אשה בגיל 40?
מה הסיכוי להצלחה?
מה ההמלצה הקלינית?

שימושים בספריות של:
Data Processing:  pandas, numpy, polars
Forecasting:      statsmodels (ARIMA), scikit-learn
Modeling:         scikit-learn, scipy
Visualization:    matplotlib, plotly, seaborn
Reporting:        jinja2, markdown
crewAI:           crewai framework with tools
