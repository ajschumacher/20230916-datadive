# 2023-09-16 DataKind DataDive

I made `20230916-six_month_retained.csv` with `20230916-002-new_6mo_retention_flag.ipynb`... I tried at first to do something fancier, but it's messy... This one just uses '6-Month Post-Placement Status Check' surveys, which unfortunately limits us to 1349 rows where we have an outcome.

 * final presentation deck: https://docs.google.com/presentation/d/1EYnXAYgZeDYQA_coiVHKP0bcWN4a8YPfkqvqkgCeOls/edit#slide=id.g27f6d49f2e6_0_146
 * event deck: https://docs.google.com/presentation/d/1ji9-3RjkWp0Ii_ImnuaGht_Is8hnQiGzB-1VeMz3tQw/edit
 * EFE prior git repo: https://github.com/DataKind-DC/EducationForEmployment
 * EFE google drive: https://drive.google.com/drive/folders/12gUAqkAADp3sxIPb7wLJnL44yt_XWUnX
 * EFE results drop doc: https://docs.google.com/document/d/1fNwUS02PC6-MBxCJgBIsqgw-5dmqZ50IiKuw9Ynm4hg/edit


---

treat ContactsProcessed.csv as the original
key determinants of job retention for 6 months or more

filter used:
<= apr 21
because data was pulled Oct 21 2022...


Employment_Start_Date, Employment_End_Date don't seem great...


---

 * RiseBoro https://riseboro.org/
     * meal delivery optimization - manage/optimize routes
     * data exploration - discovery/augmentation on seniors
 * World Vision https://www.worldvision.org/
     * identify program risks to avoid "wasted" funding
 * Hildreth Institute https://www.hildrethinstitute.org/
     * complaints from student loan people
 * National Bells Festival https://www.bells.org/
     * database of bells / map
 * Education for Employment (EFE) https://www.efe.org/
     * ongoing (last year too) MENA job placement (and keeping) thing
     * success is job retention - 6mo, 9mo, 1yr
     * Tunisia, Morocco, Egypt - what works best by country, gender
     * correlations, variable importance
     * exploratory dashboard, with filters by participant features
     * descriptives: do employment outcomes vary for males and females?
     * program value-added (predictive models?)
     * 7k students?
 * The Opportunity Project https://opportunity.census.gov/
     * improving access to electrical for climate resilience


---

```bash
pyenv install 3.11.5
pyenv virtualenv 3.11.5 datadive
pyenve local datadive
pip install matplotlib pandas scikit-learn numpy scipy jupyter statsmodels
pip freeze > requirements.txt
```
