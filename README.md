# Assignment2
Comp5349 Assignment2
Group Member: Jiakun Yu, Zezheng Zhang, Yihong Wang, Yue Yang
The code normally runs in EMR Jupyter Notebook or any Linux system with enviroment that can load Hadoop, Spark, Tensorflow and Tensorflow Hub.

## EMR Configuration:
### Software:
Release: emr-5.23.0 with Hadoop 2.85, Spark 2.4.0, Livy 0.5.0, TensorFlow 1.12.0

Software Setting:
[{"configurations":[{"classification":"export","properties":{"PYSPARK_PYTHON":"/usr/bin/python3"}}],"classification":"spark-env","properties":{}},{"configurations":[{"classification":"export","properties":{"PYSPARK_PYTHON":"/usr/bin/python3"}}],"classification":"yarn-env","properties":{}},{"classification":"spark","properties":{"maximizeResourceAllocation":"true"}}]

### Hardware Configuration:
1 Master with m4.2xlarge Instance type
2 Core with m4.2xlarge Instance type

### Bootstrap Actions:
sudo yum -y install git
sudo pip-3.6 install --quiet tensorflow-hub 
sudo pip-3.6 install --quiet numpy
sudo pip-3.6 install --quiet nltk
sudo python -m nltk.downloader -d /usr/share/nltk_data punkt
