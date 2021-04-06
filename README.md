# Installation
The model requires several tools to be installed, which are:  
* MCL: https://www.micans.org/mcl/
* Python 3.6.7
* Pytorch
* the requried packages in the "requirements.txt"  
  ```
  # pip install -r requirements.txt
  ```

# Usage Demo
**Note: You should enter into the code root directory ("/Model/") of the model.** The sample data have exist in the code directory ("/Model/datas/0_Orig"). 
1. Set the configuration file. The file "config.ini" exists in the directory "/Model/datas".
    ```
    PARAMETER
      -BetAtomDist           - the threshold that determines whether there are edges between residues (default: 8.0)
      -alpha                 - the hyperparameter of the weight formula (default: 0.6)
      -thet                  - the hyperparameter of the contrast weight formula (default: 5)
      -gamma                 - the hyperparameter of the contrast weight formula (default: 1)
      -thresh                - the threshold of the boundary edge weight (default: 0.5)
      -clusterMinSize        - the minimum number of nodes in a cluster (default: 3)
      -min_num_Epitopes      - the minimum ratio of epitope residues in the epitope cluster (default: 0.3)
    ```
2.  Run the program. The command lines are as follows:
    ```
    # python ./script/Main.py
    ```
    The results are stored in the directory "./datas/9_Adjust".  

                

