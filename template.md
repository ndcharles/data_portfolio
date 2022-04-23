<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <title>Ndcharles Nweke Data Portfolio</title>

    <link rel="stylesheet" href="stylesheets/styles.css">
    <link rel="stylesheet" href="stylesheets/pygment_trac.css">
    <meta name="viewport" content="width=device-width">
    <!--[if lt IE 9]>
    <script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
  </head>
  <body>
    <div class="wrapper">
      <header>

        <img align="middle" src="images/logo.png" alt="Logo" />

        <h1><a href="#">Ndcharles Nweke</a></h1>
        <p>Data Scientist | Machine Learning | Growth Marketing <br><br>

    An engineering graduate who is now in data science/ML. An awesome journey so far🙌. My interests are in real-life applications of data science/ML to business to tackle every day problems. <br><br>
    Let's Connect<br>
    <a href="https://linkedin.com/in/nndcharles">LinkedIn</a> | <a href="https://twitter.com/nndcharles">Twitter</a> | <a href="https://ndcharles.github.io">Blog</a><br>
    <a href="https://drive.google.com/file/d/1K_CintIw3UXhQ-qg75Jtv5SZaQnoP0RF/view?usp=sharing">View my Resume</a><br>
    
		</p>
      </header>


      <section>
        <h1>My Data Science Portfolio</h1>
		<hr>
        <p><em>View the <a href="http://github.github.com/github-flavored-markdown/sample_content.html">source of this content</a>.</em></p>

      </section>
      <footer>
<!--        <p><small>Hosted on GitHub Pages &mdash; Theme by <a href="https://github.com/orderedlist">orderedlist</a></small></p>
-->
      </footer>
    </div>
    <script src="javascripts/scale.fix.js"></script>
  </body>
</html>




<!-- Project pages  -->
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <title>Ndcharles Nweke Data Portfolio</title>

    <link rel="stylesheet" href="../assets/styles.css">
    <link rel="stylesheet" href="../assets/pygment_trac.css">
    <meta name="viewport" content="width=device-width">
    <!--[if lt IE 9]>
    <script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
  </head>
  <body>
    <div class="wrapper">
      <header>

        <img align="middle" src="../images/logo.png" alt="Logo" />

        <h1><a href="../index.html">Ndcharles Nweke</a></h1>
        <p>Data Scientist | Machine Learning | Growth Marketing <br><br>

    An engineering graduate who is now in data science/ML. An awesome journey so far🙌. My interests are in real-life applications of data science/ML to business to tackle every day problems. <br><br>
    Let's Connect<br>
    <a href="https://linkedin.com/in/nndcharles">LinkedIn</a> | <a href="https://twitter.com/nndcharles">Twitter</a> | <a href="https://ndcharles.github.io">Blog</a><br>
    <a href="https://drive.google.com/file/d/1K_CintIw3UXhQ-qg75Jtv5SZaQnoP0RF/view?usp=sharing">View my Resume</a><br>
    
		</p>
      </header>


   <section>
     <h1>Exploratory Data Analysis on Titanic Dataset</h1>
<hr>
<p>Exploratory data analysis (EDA) is an important pillar of data science. It is an important step required to complete every project regardless of type of data you are working with. Exploratory analysis gives us a sense of what additional work should be performed to quantify and extract insights from our data.</p>

<p>In this project I went through the general data analysis process using pandas, numpy, seaborn and matplotlib.</p>

<h2> Method</h2>
<p>We were provided data from <a href="https://www.kaggle.com/c/titanic/data">Kaggle</a> which contains information of all the passengers aboard the RMS Titanic, which unfortunately was shipwrecked. The data description is given below:</p>
<ul>
<li> Passengerld: Unique Id of a passenger</li>
<li> Survived: If the passenger survived(0-No, l-Yes)</li>
<li> Pclass: Passenger's Class (1 = first, 2 = second, 3 = third)</li>
<li> Name: Name of the passenger</li>
<li> Sex: Male/Female</li>
<li> Age: Passenger's age in years</li>
<li> SibSp: No of siblings/spouse aboard</li>
<li> Parch: No of parents/children aboard</li>
<li> Ticket: Ticket Number</li>
<li> Fare: Passenger's Fare</li>
<li> Cabin: Cabin nunber</li>
<li> Embarked: Port of Embarkment (C = Cherbourg; Q = Queenstown; S = Southanpton)</li>
</ul>

<p>The first step after importing the data was to preview the details therein. This is by checking the columns. Previewing the dhead of the data. And taking a 5-number statistical summary.</p>

<h2>Univariate Analysis</h2>
<p>There are 9 categorical variables and 3 numerical variables. A bar plot function was created to plot the categorical variables and a histogram function for the numerical variables.</p>

<img src="../images/barplot.jpg" alt="bar_plot"/>

<img src="../images/hist.jpg" alt="histogram"/>

<br>

<h2>Bivariate Analysis</h2>
<p>The aim here is to dig deeper into the dataset. To answer questions such as:</p>
<ul style="list-style-type: '-- ';">
<li> How many passengers with a sibling or spouse aboard survived?</li>
<li> How many males and females survived?</li>
<li> How many of the passengers survived in each passenger class?</li>
<li> What is the survival rate of passengers with a parent or child(ren) aboard?</li>
<li> What is the survival rate with regards to their age?</li>
</ul>

<img src="../images/bivariate.jpg" alt="bivariate"/>

<p>From the above figure (left to right) we can deduce that:</p>
<ul>
<li> The lesser the number of spouse or sibling one has, the higher their chances of survival.</li>
<li> More females survived while twice that number of men did not survive.</li>
<li> More passengers in the lower class did not survive, more of the upper class did survive while the middle class fared moderately. </li>
<li> More passengers came without a parent or child(ren). There was more death recorded for those without a parent or child and half of those survived.</li> 
<li> More of the passengers onboard are in their mid-twenties. The highest death was recorded for that population. They also survived more.</li>
<li> From the plot of sibling/spouse and parent/children, it can be shown that majority of the population came alone. </li>
</ul>

<h2>Missing Values</h2>
<p>A quick check on the data for missing values shows that Age is missing a couple of values (177). We have a lot of missing values in the Cabin column (687). And only 2 missing in Embarked column. The exact values missing were be gotten using .isnull().sum().</p>

<img src="../images/missing.jpg" alt="missing_values"/>

<p>The following approaches were taken to treat the missing values:</p>
<ul>
<li> Fill in the missing Age value instead of dropping NA. Replacing all Age null values with the average of their respective Pclass.(Pclass, Age)(1, 38)(2, 29)(3, 25).</li>
<li> Drop the Cabin column and the two null values in Embarked column.</li>
</ul>

<h2> What we have done</h2>
<ul>
<li> Imported our data</li>
<li> Explored its head, columns and statistical summary</li>
<li> Perform univariate and bivariate analysis</li>
<li> Find and replace missing values using average</li>
<li> Also dropped some columns and rows.</li>
</ul>

<p><a href="https://github.com/ndcharles/SGA08_DATASCI/blob/master/titanic_dataset.ipynb">View project on GitHub</a></p>

<br>
<p><a href="../index.html">Back to Portfolio</a></p> 
<hr>
<a href="https://www.github.com/ndcharles">View my GitHub profile</a> | <a href="https://www.ndcharles.github.io">Read the Blog</a>

      </section>
      <footer></footer>
    </div>
    <script src="../assets/scale.fix.js"></script>
  </body>
</html>


