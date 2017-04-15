MapReduce Test using MiniCLuster
================================
hadoop-mini-clusters provides an easy way to test Hadoop projects directly in your IDE, without the need for a full development cluster or container, It allows the user to debug with the full power of the IDE.

Project Source
--------------
Contains:
    * `BasicWordCount.java`: simple MapReduce Hadoop job for the mini-cluster test.
    * `BasicMRTest.java`: unit test for MR job in mini-cluster

Steps
-----
    * Setup the mini-cluster inside the setUp function, with HDFS path in the configurations
    * Test the cluster, by initialize the input and output folders for the job.
    * Run the job in the mini-cluster
    * Check the job results in the output folder
    * Shut down the cluster
    
References
----------
    * [MiniMRCluster blog](http://grepalex.com/2012/10/20/hadoop-unit-testing-with-minimrcluster/)
    * [MR mini-cluster test](https://github.com/bobfreitas/minicluster-mr2)
    * [MiniCluster Wrapper](https://github.com/sakserv/hadoop-mini-clusters) 

Run Test
--------
mvn test

 