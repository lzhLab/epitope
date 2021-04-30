# Installation
The model requires several tools to be installed, which are:  
* MCL: https://www.micans.org/mcl/
* Python 3.6.7: https://www.python.org/downloads/release/python-367/
* Pytorch: https://pytorch.org/get-started/locally/
* the requried packages in the "requirements.txt"  
  ```
  # pip install -r requirements.txt
  ```

# Usage Demo
**Note: The model needs to be executed in the root directory (i.e. "/Model").** The sample data have existed in the directory "/Model/data/0_Orig". 
1. Set the configuration file. The file "config.ini" exists in the directory "/Model/data".
    ```
    PARAMETER
      -BetAtomDist           - the threshold that determines whether there are edges between atoms (default: 8.0)
      -alpha                 - the hyperparameter of the weight formula (default: 0.6)
      -thet                  - the hyperparameter of the contrast weight formula (default: 5)
      -gamma                 - the hyperparameter of the contrast weight formula (default: 1)
      -threshold             - the threshold of the boundary edge weight (default: 0.5)
      -clusterMinSize        - the minimum number of nodes in a cluster (default: 3)
      -min_num_Epitopes      - the minimum ratio of epitope residues in the epitope cluster (default: 0.3)
    ```
2.  Run the program. The command line is as follows:
    ```
    # python ./script/Main.py <pdb_id> <chain_name>
    ```
    For example:
    ```
    # python ./script/Main.py 1A14 N
    ```
    The result is stored in the directory "./data/Results", i.e.:
    ```
    1A14N.clu
    ```


