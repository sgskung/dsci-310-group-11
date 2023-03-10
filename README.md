# Wine Quality Predictor

Authors: Anthony Huang, Christina Pan, and Justin Kung

## About
In this project we attempt to build a classification model which can use chemical ingredients of wine to predict the quality of wine.
Among all of mour models, the SVC RBF model obtained a best score of 0.76, which is not sufficient to accurately predict wine quality based on its chemical qualities. 
While the lower accuracy score is not ideal, it is expected. 
Errors in the predictions may be due to the limitations of the methods used; however, it is likely also due to the varying preferences of the individuals surveyed to obtain the data.
The standards and qualities of wine are all determined by people and even though there may be experts that know the field, quality is still a subjective measurement and experts will still have bias in their judgments.

Although there are several limitations to the methods used in this project, there may still be use for machine learning algorithms within the realm of predictions of wine quality. Primarily, it could still be useful in more targeted marketing techniques or finding ideal wines for more specific consumer groups.

The data set that was used in this project is the red wine dataset is created by Paulo Cortez, University of Minho (2009). 
It was sourced from the UCI Machine Learning Repository and can be found [here](https://archive.ics.uci.edu/ml/datasets/wine+quality), specifically [this file](https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv). 


## Usage

To replicate the analysis, install Docker and run the Docker application. Then clone this GitHub repository and build a docker container with the dockerfile included in this repository by:

1. Navigating to the local repository that holds the 'Dockerfile' for this project.

2. Running the following commands in the unix shell
```
docker build -t wineclass .
```
```
docker run -v $(pwd):/app -p 8888:8888 wineclass
```
3. Runnning these two commands in the unix shell will generate a file called report.html that you can view in any browser application (e.g. Chrome, Firefox).

4. Open 'report.html' and view the report.


## Dependencies:
* Python 3.10 and Python packages:
  - altair==4.1.0 
  - numpy==1.24.2 
  - pandas==1.5.2 
  - matplotlib==3.6.3 
  - scikit-learn==1.2.1 
  - ipython==8.8.0
  - pytest==7.2.2
  - jupyter==1.0.0


## Licences: 
The Wine Quality Predictor materials here are licensed under the MIT License.

## Reference:
* Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009) Modeling wine preferences by data mining from physicochemical properties. Decision Support System 547-553. https://doi.org/10.1016/j.dss.2009.05.016
