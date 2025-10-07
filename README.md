# Training-Data-Analysis---French-Regions

This project is an R Notebook that analyzes professional training data from the Mon Compte Formation platform. The goal is to clean, transform, and visualize the data to answer several analytical questions.

The main dataset, moncompteformation_formations_engagees.csv, contains information about training sessions, such as the number of enrollments, the total cost, the average price, the region and department where the training took place, and the validation date. Another dataset, fr_population.region.departement.csv, provides population data for French regions and departments, which is used to calculate costs per inhabitant.

The analysis follows several steps. First, duplicated rows in the dataset are identified. Then, a new column called prix_total is created to calculate the total price per training, and it is compared with the total amount actually spent (montant_engage). Some training labels are renamed for clarity, for example, "Yoga" is changed to "Cours de yoga".

Next, the total spending per department is calculated, with the ability to filter for specific departments such as Paris. The analysis also focuses on 2022, counting the number of trainings validated per region and calculating the total spending per region. By merging the population data, the cost per inhabitant per region is calculated.

Finally, the analysis looks at training dossiers with the status "Clos" (closed) and calculates the percentage of trainings that were fully completed.

The project uses R with packages such as dplyr and stringr. The notebook is designed to be run in RStudio. To reproduce the analysis, the datasets should be placed in the same folder as the notebook, which can then be opened and executed cell by cell.

This notebook provides a clear overview of training data, spending, regional differences, and completion rates, helping to better understand the impact and distribution of professional training programs in France.
