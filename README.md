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
My second competition, a solo one.	:grinning:

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
- [Anaconda](https://www.anaconda.com/distribution/)

## Usage
Few ways to run these notebooks interactively:

### Jupyter Notebook
<details>
<summary>Details</summary>
  
1. Download this repository in a zip file by clicking [here](https://github.com/y33-j3T/Kaggle-PUBG-Finish-Placement-Prediction/archive/master.zip) or execute this from the terminal: 
```
git clone https://github.com/y33-j3T/Kaggle-PUBG-Finish-Placement-Prediction.git 
```
2. Download the datasets at [competition website - data](https://www.kaggle.com/c/pubg-finish-placement-prediction/data).
3. Put both downloads in the same directory and unzip them.
4. For cleanliness, create a new folder `input` and put the datasets (with `.csv` extensions) into it.
4. Open Anaconda Prompt.
5. Navigate to the **repository folder** with
```
cd [path address]
```
6. Create a virtual environment with
```
conda create -n [environment name] python=3.7
```
7. Activate the environment with 
```
activate [environment name]
```
8. Install the required dependencies with
```
pip install -r requirements.txt
```
9. Execute Jupyter Notebook from the command line or terminal with
```
jupyter notebook
```
10. Click on files with `.ipynb` extension on the Jupyter Notebook dasboard and enjoy!
11. When you're done, deactivate the virtual environment with 
```
deactivate
```

</details>

### Google Colab
<details>
<summary>Details</summary>

1. Download the datasets at [competition website - data](https://www.kaggle.com/c/pubg-finish-placement-prediction/data).
2. Put all downloads in the same directory and unzip them.
3. For cleanliness, create a new folder `input` and put the datasets (with `.csv` extensions) into it.
4. Click on any model you want work with at the [**Model Deployment**](#Model-Deployment) section.
5. Copy the link of the page and paste it into the search bar of a new page.
6. Replace `https://github.com` with `colab.research.google.com/github` and hit <kbd>enter</kbd>.
7. Go to the sidebar, click on **Files** > **Upload**.
8. Upload all contents in the `input` folder.
9. You may now run the notebook.
10. Once you are done, remember to save the notebook somewhere.
  
</details>

### Kaggle Kernels
<details>
<summary>Details</summary>
  
1. Download this repository in a zip file by clicking [here](https://github.com/y33-j3T/Kaggle-PUBG-Finish-Placement-Prediction/archive/master.zip) or execute this from the terminal: 
```
git clone https://github.com/y33-j3T/Kaggle-PUBG-Finish-Placement-Prediction.git 
```
2. Unzip your download.
3. Go to [competition website - kernels](https://www.kaggle.com/c/pubg-finish-placement-prediction/kernels).
4. Click on **New Kernel**.
5. Select **Notebook**.
6. Click on **File** > **Upload Notebook**.
7. Upload any file with `.ipynb` extension that you want to work with and enjoy!
8. Once you are done, remember to click on **Commit**.

</details>


## Exploratory Data Analysis
- *work in progress*

## Model Deployment
- [Random Forest model](./pubg-finish-placement-prediction-rf.ipynb)
- [XGBoost model](./pubg-finish-placement-prediction-xgb.ipynb)
- [Ensemble model](./pubg-finish-placement-prediction-ensemble.ipynb)

## Contributing
Please refer to [CONTRIBUTE.md](./CONTRIBUTE.md) for details. :heart_eyes:

## License
Kaggle PUBG Finish Placement Prediction is released under the [MIT License](./LICENSE).
