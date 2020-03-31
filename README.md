HDFS Contents Manager for Jupyter Notebooks
===========================================  

A contents manager for Jupyter that stores files in Hadoop File System (HDFS)


Install
-------

1) Install pyarrow



Run
----

You can use command line arguments to set HDFS related configurations



  jupyter-notebook --NotebookApp.contents_manager_class='hdfscontents.hdfsmanager.HDFSContentsManager' \
        --HDFSContentsManager.hdfs_namenode_host='localhost' \
        --HDFSContentsManager.hdfs_namenode_port=9000 \
        --HDFSContentsManager.root_dir='/user/'
        


Alternatively, first run:
``` 
  jupyter-notebook --generate-config  
```  
to generate a default config file. Edit and add the HDFS related configurations in the generated file. Then start the notebook server.
```  
  jupyter-notebook
```
