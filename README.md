# Querying Infinite Process Models
## Master's Thesis 



File Structure of the GitLab repository:

In the root folder we have the ```Final_Thesis_Algorithm_Implementation.ipynb```
 which contains the code, the ```requirements.yaml``` containing the complete environment description we have used in anaconda in order to run our files, the ```README.md``` and ```my_petri_net.pnml``` to use as a toy-model. 
 The dataset folder holds the provided datasets that we have mined using the alpha miner in ProM, further details on the data can be found on the thesis itself.

For the execution: 
Change the path variable (second cell of the notebook) to the desired Petri net path.
Run all the cells of the Jupyter Notebook 
```Final_Thesis_Algorithm_Implementation.ipynb``` sequentially (Run All).

In the last two cells the printed statements will return the average query time and the Formula Truth % for all the executions.
It should be noted that if the total runtime of the algorithm is  &lt;1ms then the time is shown as zero. This is exactly why when we run the code with the toy-model (```my_petri_net.pnml```) the average query time is shown as zero.
This happens due to the limitations of the method we use to count the time, but is not an issue with larger Petri nets (like the ones we used to test the algorithm with), where checking all the possible combinations takes multiple seconds/minutes.
