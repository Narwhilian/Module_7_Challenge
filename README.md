# ETF_App

This application that analyzes the performance of an ETF composed of four securities (GDOT, GS, PYPL, SQ) and deploys the results as a web application

---

## Technologies

This project uses the Python Programming language in a Jupyter Notebook as well as the following libraries
    
    - numpy
    - pandas
    - hvplot
    - SQLalchemy


---

## Installation Guide

To install you will want to pull the entire ETF_App folder from github including its subfolder
    
    * Subfolder
        * etf.db (the database containing all of the information we use to analyze the portfolio)
        * etf_analyzer.ipynb (the jupyter notebook itself)
        * ReadMe (This file)


---

## How it works

1) First the user will open the etf_analyzer.ipynb notebook in the ETF_App folder
2) Then the user will simply run each cell in the notebook in order to get its output

    i) The app will load the pypl data into a dataframe from the database using a SQL query
    
    ii) Then it will chart the daily pypl returns from the newly created dataframe as well as calculate and chart the cumulative returns of pypl
    
      ![PYPL returns](https://user-images.githubusercontent.com/84096312/126021288-89534f65-3574-4a3f-894c-ccff30042a5a.png)
      ![pypl cumulative](https://user-images.githubusercontent.com/84096312/126021330-8221d035-0c31-4439-92e9-1375bd0aeca7.png)

    
    iii) Then it will identify the days where pypl had the best historical returns and rank them

    
    iv) It will then concat the tables holding each of the stocks in the database and create a new variable that is the mean of their combined daily returns to act as the ETF portfolio. It will then tell you the portfolios average annual return as well as its total cumulative return.
    
    
    v) Then it will plot the portfolio cumulative return
    
      ![port cumulative return](https://user-images.githubusercontent.com/84096312/126021444-1ccae54d-8299-4bb6-bf0d-de950b3cbb3f.png)

    vi) Finally it will deploy the app as a web app using the voila package
    
      

    https://user-images.githubusercontent.com/84096312/126021503-297d9f2e-3b52-4617-a839-8d322d5b40ec.mp4




---

## Usage

Overall it should be a very simple application to use, all you need to do is open the etf_analyzer.ipynb app in the ETF_App folder and run each cell in order


---

## Contributors

Colin Benjamin

Linkedin: [Colin Benjamin](https://www.linkedin.com/in/colinbenjamin/)
    
email: cbenjamin33@gmail.com

---

## License

MIT
