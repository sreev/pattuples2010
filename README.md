# Pattuples production from 2010 data

The exercise produces tuples created following the Physics Analysis Toolkit (pattuples) from the 2010 AOD data.

You need to work in a VM properly contextualized for CMS.

In order to run the PAT_data_repo.py to generate the pattuples 
you need to create a working area and source a proper CMS environment.

## Creating the Working Area

This step is only needed the first time.

```
cmsrel CMSSW_4_2_8
cd CMSSW_4_2_8/src
```

## Sourcing the environment 

This step is needed each time you want to run the exercise.

```
source /cvmfs/cms.cern.ch/cmsset_default.sh
cd CMSSW_4_2_8/src
cmsenv
```

## Producing the pattuples

Clone the repo:

```
git clone https://github.com/ayrodrig/pattuples2010.git 
cd pattuples2010
```

Run: 

```
cmsRun PAT_data_repo.py 
```

In this case the pattuples production was splitted in 6 executions per dataset (Mu and Electron);
each runs over aprox. 500 files. An example of the partition is found in the Mu2010data* and Electron2010data* files.

