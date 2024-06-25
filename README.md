## Detecting Collaborative Scanners based on Shared Behavioral Features

This project hosts the code and intermediary data used during the [CSE3000 Research Project](https://github.com/TU-Delft-CSE/Research-Project) course at [TU Delft](https://github.com/TU-Delft-CSE), in Q4 23/24. 
The work uses network telescope data with HDBSCAN and DBSCAN to cluster collaborative scanners based on shared behavioral features, such as the median inter-packet time, tool, IP generation algorithm, scan length, source/destination ports.

### Notice 
For obvious privacy reasons, the repository cannot be re-run without proper access to the TU Delft database, which has been redacted. Only some of the functionality is available without access.

### File Structure 

| Path        | Description |
| ----------- | ----------- |
| /day_data   | Data for each day between 1st and 20Feb 2024       |
| /results    | Raw results from each algorithm run        |
| /analysis   | Data resulted from further analysis, with heavy hitters/post-processing/stats |
| day_data_writer.ipynb | Notebook to generate data for each day |
| day_data_aggregator.ipynb | Notebook that aggregates all data for all days in one collection |
| model_training.ipynb | Notebook used to train the models |
| group_validation.ipynb | Conducts group validation by calculating heavy hitters and overlaps |
| post_processing.ipynb | Applies a greedy algorithm to find sub-groups with no overlaps |
| plotter.ipynb | Code for plots |
