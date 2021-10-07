## Project Process

1. Create data folder on shared drive and put data into a `raw` subfolder, create `processed`, and `final` subfolders as well.
1. Create repository on github for code, update ReadMe with information about the project (stakeholders, data sources, description, goals, maintainers).
1. Download repository onto aws `GISUSER_?` machine.
1. Explore data in QGIS or ArcGIS.
1. Exploratory data cleaning steps are written in jupyter notebooks, but when they're finalized, we transfer them to data pipelines.
1. Create a `requirements.txt` file with all libraries needed for project (arcpy, geopandas, tqdm, etc.), maybe enforce conda environments
1. Let's not commit any code to the master branch ever. Let's make sure we are working branches and making PRs, and getting code reviewed by a peer before pushing into master.

   - `git checkout -b <branchname>`

   - `git add <fileame>`

   - `git commit -m 'message'`

   - `git push`

1. When finish a feature or a work sprint, make a pull request into the master branch and request a code review. Someone other than you reviews the code (if Rohit pushes, Mushtaaq reviews, if Mushtaaq pushes, Rohit reviews).
1. If the code looks good, push into `main` branch, otherwise offer feedback, and do another code review cycle
1. Write code for storing data in s3 buckets.
