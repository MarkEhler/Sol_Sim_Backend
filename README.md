# Sol_Sim_Backend
ToC
<ul>
  <li> Data_collection.ipynb - Scripts for collecting and merging various data used for this project </li>
  <li> Ensemble_Method.ipynb - Iterative notebook for further data processing and algorithm selection </li>
</ul>
<br>
The roots of this project start in good data practices.  Several datasets were merged to create a robust collection of over 2 million samples.  Those 2m were wittled down over the course of iterative selective process.  Certain features had to be dropped, others were filled in with known values that wern't represented.  The final [Sol-Sim features](https://i.imgur.com/V82SBdU.png) was a narrow list with room to build upon should the model warrent more time and effot.
<br>
In the Ensemble_Method.ipynp module, several versions of the data set were check against several grid search models tested with a cross validation using 3 or more suffles.  In the end XGBoost preformed best.  The notebook does not run strictly in order, rather several cells are meant to be used as options to be ran the model option cells below.  The final model boasted and accuracy of 77 Watts/Meter^2.  The distribution of [Watts/Meter^2 of all training data](https://i.imgur.com/HYj9cqK.png) combined with the usage of this data leaves me with a comfortable model that I found resonsive to the features that I care about ie weather, time of year, time of day.



