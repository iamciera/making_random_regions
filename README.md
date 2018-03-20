# README.md 

## About

**Purpose**: We want to find random 2kb regions that will act as "control" for statistical tests. Are the properties that are found in random 2kb regions different then those that are represented with the kvon dataset. 

Goal is to have an output file in bed format.## Authors

Team Data Exploration. 

## To Do

- [ ] Double check `cleanedFlybaseBetweenGenes_17July2017.BED` ranges.  Do they make sense?
- [ ] Retrieve random number between start and end regions in the `cleanedFlybaseBetweenGenes_17July2017.BED` file
- [ ] Choose random regions and allow resampling
- [ ] You go up or down 2kb
  - [ ] Is the region at least 2KB
    - yes, continue
    - no, don't use
   - [ ] Make sure it doesn't hit the start or end
- [ ] Make sure it does not overlapp with previous Kvon data sets.
- [ ] Make sure it does not overlap in promoter regions ect.
- [ ] Visualize

## Files
- data/input/`dmel-all-r6.13.gtf`: This is a file designating all the annotated regions of the fly genome. file came from here: [ftp://ftp.flybase.org/genomes/dmel/current/gtf/](ftp://ftp.flybase.org/genomes/dmel/current/gtf/) This was used to create `cleanedFlybaseBetweenGenes_17July2017.BED`
-  data/input/`cleanedFlybaseBetweenGenes_17July2017.BED`: This is a file that labels every gene region in the fly genome. This was cleaned up a bit using `1.cleanUp_flybase.Rmd`
-  data/input/`1.kvon_redfly_BED4_full_17May2016.bed`: This is the bed file that was used to retrieve all the sequence data is located on [Google Drive](https://drive.google.com/open?id=1kAh9NPg0gin4KIYvdz2Czi1LCQ2Js06X).  This is used to make sure the random regions collected do not overlap with Kvon regions.

## Data Management

See [`data_management.md`](https://github.com/DiscoveryDNA/team_data_exploration/blob/master/data_managment.md)


