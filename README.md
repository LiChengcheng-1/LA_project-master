# Table of content 
- [The Duck's School](#headers)
- [Dataset Description](#headers1)
- [Implementation Technologies](#headers2)
- [App Structure](#headers3)
- [Visualization](#headers4)
- [To deploy the project](#headers5)
- [Members](#headers6)

<a name="headers"/>

<img src="https://github.com/LiChengcheng-1/LA_project-master/blob/master/LA_project-master/static/images/logo2.png" align= " right">
<br>
<br>
<a href="https://youtu.be/2ErSRCsd7qc">A Youtube video shows a demo</a>


# The Duck's School
Welcome to The Duck’s School App, Which help students to choose their ideal course based on many approaches.
In the Duck’s School, we use information about subjects that students have studied and other students' subjects by employing the Recommended Systems approach, as well as the non-Personalized approach by visualizing different attributes of courses to students to assist them compare between the courses. The Ducks' School is user-friendly for students in all disciplines, not just IT.
The Duck’s School was developed as part of a Learning Analytics lecture project at Duisburg – Essen University.


<a name="headers1"/>

# Dataset Description
For this project we created our own dataset based on infromations collected from the [Open University Learning Analytics Dataset
](https://analyse.kmi.open.ac.uk/open_dataset#about).From 2013 to 2014, the dataset contains information about students, courses, and their activities.
These informations are:
* Lecture name
* Lecture pass rate
* Students'informations,such as age, gender, region and so on
* Scores
* Previous attempts


Needed libraries:

```ruby
* Pymongo
* Pandas
```

<a name="headers2"/>

# Implementation Technologies
The following technologies are used in this project:

* Data preprocessing
  + Pandas
  + Numpy
* Front-End
  + Website
    + Flask templates
    + JS
    + AJAX
    + CSS
    + HTML
  + Visualisation
    + Bokeh
* Back-End
  + Web Server
    + Flask
  + Machine Learning 
    + Recommender Systems: Recommenders from Microsoft
  + Database
    + mongoDB
* Other Tools
  + Jupyter Notebook
  + Pycharm

<a name="headers3"/>

# App Structure
The project has the following structure:

App (Couses):
  + BarVis.py
  + DataVis.py
  + PieVis.py
  + app.py
  + config.py
  + finalized_model.sav
  + models.py
  + package.json
  + static (folder)
    + css (folder)
    + fonts (folder)
    + images (folder)
    + js (folder)
  + templates (folder)  (contian the pages of the Web App)


## Machine Learning Pipeline
* <a href="data/nlp/cleaner.py">Data preprocessing</a>
  + Remove html Tags, punctuations, stop words from the <i>description</i>, <i>learning_targets</i> and <i>pre_qualifications</i> columns, 
  + Lemmatization
  + Merging the 3 columns to form a main column
* <a href="data/machine_learning/recommandation/content_based/gensim_d2v.py">Machine Learning Algorithm</a> 
  + Word tokenization
  + Data Filtering based on Input of the user (language, study course)
  + Document Tagging
  + Model Building (Doc2Vec)

<a name="headers4"/>

# Visualization
All visualization charts are created with the tool Bokeh, and there are three types of plots, and some Visualization examples are shown below.
+ <a href="https://bokeh.org/"> Bokeh </a>
+ Bar Chart
<img src="https://github.com/LiChengcheng-1/LA_project-master/blob/master/LA_project-master/static/images/BarChart.png">

+ Pie Chart
<img src="https://github.com/LiChengcheng-1/LA_project-master/blob/master/LA_project-master/static/images/PieChart.png">

+ Grouped Bar Chart
<img src="https://github.com/LiChengcheng-1/LA_project-master/blob/master/LA_project-master/static/images/GroupedBarChart.png">

<a name="headers5"/>

# To deploy the project
First you need to install below requirements:
+ <a href="https://www.jetbrains.com/pycharm/download/#section=windows">Download PyCharm</a> or your preferred IDE.
+ <a href="https://www.python.org/downloads/">Download latest version of Python</a>

After configuring the python inside your IDE you need to install this project from this repository. 

Then you need to install below requirements on our system:
  * [Flask](https://flask.palletsprojects.com/en/1.1.x/installation/#install-flask) == 2.1.2
  * [Pandas](https://pypi.org/project/pandas/) == 1.5.3
  * [NumPy](https://numpy.org/) == 1.24.2 
  * [Bokeh](https://docs.bokeh.org/en/latest/docs/first_steps/installation.html) == 3.0.3
  * [PyMongo](https://pymongo.readthedocs.io/en/stable/installation.html) == 4.3.3
  

<a name="headers6"/>

# Members
* Hong Yang
* Chengcheng Li
* Chau Le 
* Zaid A.R Abdulmohsin
* Ahmed Abdelbary
* Saba Darbandi


