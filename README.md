# The directory structure of code
Model  
　　├─datas  
　　│　│　config.ini　**This is the configuration file.**  
　　│　│　  
　　│　├─0_Orig　**The directory contains the preprocessing PDB data.**  
　　│　│　├─antigens  
　　│　│　│　　　  
　　│　│　├─epitopes  
　　│　│　│　　　  
　　│　│　├─pdbchain  
　　│　│　│　　　  
　　│　│　└─RotationAminoInfos  
　　│　└─filelist　**The directory contains the name list of PDB data.**  
　　│　　　　　  
　　└─script　**The directory contains this model codes.**  
　　　　│　Main_1.py　**The first step of main program: Overlapping subgraph clustering.**  
　　　　│　Main_2.py　**The second step of main program: Training classificaton model.**  
　　　　│　__init__.py  
　　　　│　  
　　　　├─AminoEdge  
　　　　│　　　GetAminoEdges_1.py  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─AminoWeight  
　　　　│　　　CalcAllAminoWeights_1.py  
　　　　│　　　GetAminoEdgeWeights_2.py  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─ExpCluster  
　　　　│　　　DMF_boundary_1.py  
　　　　│　　　DMF_ExpLMetric_2.py  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─ExtractFeatures  
　　　　│　　　Classification_2.py  
　　　　│　　　GetGraphOrigDatas_1.py  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─MarkovCluster  
　　　　│　　　FilterCluster_2.py  
　　　　│　　　RunMcl_1.py  
　　　　│　　　__init__.py  
　　　　│　　　  
　　　　├─methods  
　　　　│　│　BaseFunction.py  
　　　　│　│　dataUtils.py  
　　　　│　│　SearchNeighbors.py  
　　　　│　│　__init__.py  
　　　　│　│　  
　　　　│　└─GCN  
　　　　│　　　　 ClassficationModel.py  
　　　　│　　　　 layer.py  
　　　　│　　　　 preprocessing.py  
　　　　│　　　　　　　  
　　　　└─NetWork  
　　　　　　　　BuildNetWork_1.py  
　　　　　　　　__init__.py  
　　　　　　　　  


　　　　　　　　　

                

