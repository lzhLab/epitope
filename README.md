# The directory structure of code
Model  
　　├─datas  
　　│　│　config.ini　**-> This is the configuration file.**  
　　│　│　  
　　│　├─0_Orig　**-> The directory contains the preprocessing PDB data.**  
　　│　│　├─antigens  
　　│　│　│　　　  
　　│　│　├─epitopes  
　　│　│　│　　　  
　　│　│　├─pdbchain  
　　│　│　│　　　  
　　│　│　└─RotationAminoInfos  
　　│　└─filelist　**-> The directory contains the name list of PDB data.**  
　　│　　　　　  
　　└─script　**-> The directory contains this model codes.**  
　　　　│　Main_1.py　**-> The first step of main program: Overlapping subgraph clustering.**  
　　　　│　Main_2.py　**-> The second step of main program: Training classificaton model.**  
　　　　│　__init__.py  
　　　　│　  
　　　　├─AminoEdge  
　　　　│　　　GetAminoEdges_1.py　**-> Step 1: Get the edge between residues.**  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─AminoWeight  
　　　　│　　　CalcAllAminoWeights_1.py　**-> Step 2-1: Calculate the edge weight between residues.**  
　　　　│　　　GetAminoEdgeWeights_2.py　**-> Step 2-2: Get the edge weight of the train data.**  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─ExpCluster  
　　　　│　　　DMF_boundary_1.py　**-> Step 5-1: Expand subgraphs by using two-stage DFM.**  
　　　　│　　　DMF_ExpLMetric_2.py　**-> Step 5-2: Continue to expand subgraphs by using L-Metric algorithm.**  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─ExtractFeatures  
　　　　│　　　Classification_2.py　**-> Step 6-2: Construct classification model.**  
　　　　│　　　GetGraphOrigDatas_1.py　**-> Step 6-1: Transform subgraph data to train data.**  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─MarkovCluster  
　　　　│　　　FilterCluster_2.py　**-> Step 4-2: Filter the subgraphs that the number of nodes are less than 3.**  
　　　　│　　　RunMcl_1.py　**-> Step 4-1: Get seed subgraphs by using MCL.**  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─methods  
　　　　│　│　BaseFunction.py　**-> Base function for residues.**  
　　　　│　│　dataUtils.py　**-> Utility classes.**  
　　　　│　│　SearchNeighbors.py　**-> The implement for searching neighbors by using KD-tree.**  
　　　　│　│　__init__.py  
　　　　│　│　  
　　　　│　└─GCN　**-> The directory contains the classes for GCN model construction.**  
　　　　│　　　　 ClassficationModel.py  
　　　　│　　　　 layer.py  
　　　　│　　　　 preprocessing.py  
　　　　│　　　　　　　  
　　　　└─NetWork  
　　　　　　　　BuildNetWork_1.py　**-> The second step of main program: Training classificaton model.**  
　　　　　　　　__init__.py  
　　　　　　　　  

　　　　　　　　  


　　　　　　　　　

                

