# About this folder

This folder contains the settings and results of the four Croudsourcing jobs
done at [CrowdFlower](http://crowdflower.com/) for establishing the benchmark.

The complete run contained 1490 sound pairs for dissimilarity judgments.
The sound pairs were all combinations between the 10 query sounds of D1
and the other 149 sounds of D1. Hence in the crowdflower data set query_id 
means the query and result_id belongs to the compared sound.
Five judges had to judge the similarity of every of these 1490 sound pairs.

The three testruns differ only marginally from the complete run.
The basic idea was first to get some qualitative feedback on why sounds are 
similar or not, but it turned out that this task is not perfectly suited for 
crowdsourcing. For the testruns only 100 rows of the 1490 were used.

## Contents

* crowdflower_similarity_verbose.pdf --> a verbose version of the similarity matrix as included in the Bachelor's thesis, but with Freesound ids instead of names and the ids of every sound in the 150 columns

* crowdflower_utils.py --> contains code used to work with crowdflower, mainly the code used for evaluation


### Every folder (Complete, Test1, Test2, Test3) contains the following files:

#### Information on settings

* ..._instructions.html --> the html file of the instructions
* ..._task.html --> the html file of the task

Note: cml elements belong to the CrowdFlower Markup Language and hence get not 
displayed in the standard html preview


#### Results

* ..._full_report.csv --> lists each individual response from contributors
* ..._aggr_all.csv --> lists the aggregated responsed on each rated sound pair
* ..._sourcedata.csv --> the original, unprocessed data thas was uploaded
* ..._testquestions.csv --> includes data only on the testquestions
* ..._contributors.csv --> information on the performance of contributors
