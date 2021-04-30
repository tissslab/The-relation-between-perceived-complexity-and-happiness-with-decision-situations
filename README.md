# The-relation-between-perceived-complexity-and-happiness-with-decision-situations

This repository contains all the code used for producing the graphs and results tables in the paper "The relation between perceived complexity and happiness with decision situations: searching for objective measures in social simulation games".

The three jupyter notebooks containg the python3 code are:
* run party simulation.ipynb
  The most important jupyter notebook: it contains the game simulations. The program allows you to change simulation settings and choose if the simulation logs should be saved to the '/logs' folder of if the moving-decisions should be saved to the '/agent learning data' folder.
  
* analyze simulation logs.ipynb
  This program retrieves the data from the log-files in the '/logs' folder and uses this to calculate the overall metrics for the five different games. Intemediary results of from this log summarisation are saved in the '/log summary' folder. The final result is saved in the file 'data/overall_simulation_results.csv'
  
* agent learning.ipynb
  This program simulates learning agents. It uses the moving-decision data from the '/agent learning data' folder to train a neural network aimed at predicting when agents have to move i.e. learning the game's rules. By giving the neural network increasing amounts of data, we are simulating the agent observing the game for an increasingly long time. The results from this program are saved in the the '/agent learning results' folder.
 
