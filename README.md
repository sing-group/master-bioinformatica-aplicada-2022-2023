# Machine Learning in Bioinformatics
> Máster en Bioinformática Aplicada a Medicina Personalizada y Salud (Curso 2022-2023)

# Scheduling

## First week

- Day 1 (01.03.2023):
	- 1/2 Theory
	- 1/2 Practice: Setting up the environment for the Hands-On practice sessions
- Day 2 (02.03.2022):
	- 1/2 Theory
	- 1/2 Theory: presentation of a real case-study (the [PolyDeep project](polydeep.org/))
- Day 3 (03.03.2022):
	- 1/2 Theory
	- 1/2 Project: Session I (project presentation and creation of work groups)

## Second week
- Day 4 (13.03.2023):
	- Practice: Hands-On (Machine Learning Basics in Python with scikit-learn I)
- Day 5 (14.03.2023):
	- Practice: Hands-On (Machine Learning Basics in Python with scikit-learn Part II)
- Day 6 (15.03.2023):
	- 1/2 Theory
	- 1/2 Project: Session II (with problem and dataset presentation)
- Day 7 (16.03.2023):
    - Project: Session III
- Day 7 (17.03.2023):
    - Project Session: IV (with results presentation)

# Theory

The theory slides are available [here](resources/theory-machinelearning.pdf).

# Practice

## Pulling the Docker images

Run the following comands to pull the Docker image for the hands-on practices:

```bash
docker pull singgroup/jupyter-machine-learning:2022-2023
```

During the hands-on sessions (Machine Learning Basics in Python with scikit-learn), we are going to use the `Breast Cancer Data` available at the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). More information about this dataset can be found [here](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names) and [here](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data).

Go to an empty folder and run the following commands to download the data: 
```bash
mkdir data

wget https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data -O data/wdbc.data

sed -i '1iid,diagnosis,radius_mean,texture_mean,perimeter_mean,area_mean,smoothness_mean,compactness_mean,concavity_mean,concave points_mean,symmetry_mean,fractal_dimension_mean,radius_se,texture_se,perimeter_se,area_se,smoothness_se,compactness_se,concavity_se,concave_points_se,symmetry_se,fractal_dimension_se,radius_worst,texture_worst,perimeter_worst,area_worst,smoothness_worst,compactness_worst,concavity_worst,concave points_worst,symmetry_worst,fractal_dimension_worst' data/wdbc.data
```

Alternatively, the file is also available [here](data/wdbc.data).

Run the following command to use the Docker image to start a Jupyter notebook with the required libraries already installed: 
```bash
docker run --rm -p 8888:8888 -v "$(pwd)":"$(pwd)" -w "$(pwd)" singgroup/jupyter-machine-learning:2022-2023
```

The `resources/notebook-ml-1.ipynb` file contains the notebook to develop during these sessions.

# Project

The information about the project is available [here](resources/PROJECT.md).

# References
- [Practical Statistics for Data Scientists: 50 Essential Concepts](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)

# Additional Resources
- Ten quick tips for machine learning in computational biology [[10.1186/s13040-017-0155-3](https://dx.doi.org/10.1186%2Fs13040-017-0155-3)]
- [LIBSVM -- A Library for Support Vector Machines](https://www.csie.ntu.edu.tw/~cjlin/libsvm/)
- [scikit-learn: machine learning in Python](https://scikit-learn.org/stable/)

