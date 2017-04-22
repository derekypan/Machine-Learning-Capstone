# Machine Learning Engineer Nanodegree
## Specializations
## Project: Capstone Proposal and Capstone Project

**Note**

The Capstone is a two-staged project. The first is the proposal component, where you can receive valuable feedback about your project idea, design, and proposed solution. This must be completed prior to your implementation and submitting for the capstone project. 

You can find the [capstone proposal rubric here](https://review.udacity.com/#!/rubrics/410/view), and the [capstone project rubric here](https://review.udacity.com/#!/rubrics/108/view). Please ensure that you are following directions correctly when submitting these two stages which encapsulate your capstone.

You will find an `open_projects` folder in these files. This will be where pre-curated capstone projects are available, should you choose to work on a project already partially designed for you. 

Please email [machine-support@udacity.com](mailto:machine-support@udacity.com) if you have any questions.

### Software Requirements
This project uses the following software and Python libraries:

- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/0.17/install.html) (v0.17)
- [XGBoost Tree] (http://www.picnet.com.au/blogs/guido/post/2016/09/22/xgboost-windows-x64-binaries-for-download/) for windows

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html).

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer.

### Code
All code for the project is provided in the "All Together".ipynb notebook file. The csv files in anime-recommendations-database.zip are required for the code to run correctly. 

### Run
Navigate to top level of repository and make sure to unzip anime-recommendations-database.zip in that directory. Then in the command line enter:

```bash
jupyter notebook "All Together".ipynb
```

This will open the jupyter notebook in your browser from which you can run all the code.

### Data

Our data comes from 76000 users of the website myanimelist.net as posted on Kaggle. It is
presented in the form of 2 separate CSV files.

**Anime.csv Features**
1) `anime_id`: id number associated with anime (numeric);
2) `name`: name of the anime (nominal);
3) `genre`: list of genre's applicable to show (nominal);
4) `type`: type of show ex. Movie, TV, OVA (nominal);
5) `episodes`: number of episodes in show (numeric);
6) `rating`: average user rating (numeric: 1-10);
7) `members`: number of memebers in the shows group/community (numeric);

**Rating.csv Features**
1) `user_id`: id number associated with some user (numeric);
2) `anime_id`: id number associated with anime, same as in Anime.csv (numeric);
3) `rating`: user rating of anime, not the same as rating in Anime.csv (numeric);