# Kaggle PUBG Finish Placement Prediction
Competition website: https://www.kaggle.com/c/pubg-finish-placement-prediction

## Contents
- [Introduction](#Introduction)
- [Installation](#Installation)
- [Usage](#Usage)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Model Deployment](#Model-Deployment)
- [Contributing](#Contributing)
- [License](#License)

## Introduction

### Competition Description
<details>
<summary>Details</summary>
  
> So, where we droppin' boys and girls?
>
> Battle Royale-style video games have taken the world by storm. 100 players are dropped onto an island empty-handed and must explore, 
scavenge, and eliminate other players until only one is left standing, all while the play zone continues to shrink.
>
> PlayerUnknown's BattleGrounds (PUBG) has enjoyed massive popularity. With over 50 million copies sold, it's the fifth best selling 
game of all time, and has millions of active monthly players.
>
> The team at PUBG has made official game data available for the public to explore and scavenge outside of "The Blue Circle." This competition is not an official or affiliated PUBG site - Kaggle collected data made possible through the PUBG Developer API.
>
> You are given over 65,000 games' worth of anonymized player data, split into training and testing sets, and asked to predict final placement from final in-game stats and initial player ratings.
>
>What's the best strategy to win in PUBG? Should you sit in one spot and hide your way into victory, or do you need to be the top shot? Let's let the data do the talking!

*from [competition website...](https://www.kaggle.com/c/pubg-finish-placement-prediction)*

</details>

### Competition Evaluation
<details>
<summary>Details</summary>
  
> Submissions are evaluated on [Mean Absolute Error](https://en.wikipedia.org/wiki/Mean_absolute_error) between your predicted `winPlacePerc` and the observed `winPlacePerc`.
>
> Submission File
> For each Id in the test set, you must predict their placement as a percentage (0 for last, 1 for first place) for the `winPlacePerc` variable. The file should contain a header and have the following format:
> ``` markdown
> Id,winPlacePerc
> 47734,0
> 47735,0.5
> 47736,0
> 47737,1
> etc.
> ```
> See `sample_submission.csv` on the [data page](https://www.kaggle.com/c/pubg-finish-placement-prediction/data) for a full sample submission.
  
*from [competition website...](https://www.kaggle.com/c/pubg-finish-placement-prediction)*

</details>

## Installation
* [NumPy](http://www.numpy.org/)
* [IPython](http://ipython.org/)
* [Pandas](http://pandas.pydata.org/)
* [Matplotlib](http://matplotlib.org/)

## Usage
To run this notebook interactively:

1. Download this repository in a zip file by clicking [here](https://github.com/y33-j3T/Kaggle-PUBG-Finish-Placement-Prediction/archive/master.zip) or execute this from the terminal: `git clone https://github.com/y33-j3T/Kaggle-PUBG-Finish-Placement-Prediction.git `
2. Install [virtualenv](http://virtualenv.readthedocs.org/en/latest/installation.html).
3. Navigate to the directory where you unzipped or cloned the repo and create a virtual environment with `virtualenv env`.
4. Activate the environment with `source env/bin/activate`
5. Install the required dependencies with `pip install -r requirements.txt`.
6. Execute `ipython notebook` from the command line or terminal.
7. Click on `Titanic.ipynb` on the IPython Notebook dasboard and enjoy!
8. When you're done deactivate the virtual environment with `deactivate`.

## Exploratory Data Analysis
Official datasets website: https://www.kaggle.com/c/pubg-finish-placement-prediction/data
- [Data Preprocessing]


## Model Deployment
- [Random Forest model](./pubg-finish-placement-prediction-rf.ipynb)
- [XGBoost model](./pubg-finish-placement-prediction-xgb.ipynb)
- [Ensemble model](./pubg-finish-placement-prediction-ensemble.ipynb)

## Contributing
Please refer to [CONTRIBUTE.md](./CONTRIBUTE.md) for details. :heart_eyes:

## License
Kaggle PUBG Finish Placement Prediction is released under the [MIT License](./LICENSE).
