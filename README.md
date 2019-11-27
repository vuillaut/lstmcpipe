# LST scripts
Scripts to ease the reduction of MC data on the LST cluster at La Palma.   


## Steps

- `onsite_mc_r0_to_dl1.py`
    - mandatory input: directory you want to analyse. e.g. 
    `/fefs/aswg/data/mc/DL0/20190909/proton/North_pointing`
    - it will create the directory structure for you
    - creates batch jobs
    - results can be found in `running_analysis`
- `onsite_mc_merge_and_copy_dl1.py`
    - to be run once all jobs from `onsite_mc_dl0_to_dl1.py` are finished
    - check that jobs finished without error from the logs
    - merge the DL1 files for training and testing
    - clean and move the `running_analysis` into `DL1` and `analysis_logs`
- `onsite_mc_train.py`
- `onsite_mc_perf.py` (TBD)
        
    
### Real Data analysis

Real data analysis is not supposed to be supported by these scripts.    