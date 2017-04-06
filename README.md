# MLB Pitchers Friend

*"Helping hitters become batters...and then sitting them back down"*

#### [Full Project Description](https://github.com/fire-ants/mlb-admin/blob/master/README.md)

## MLB Queen Ant
The **MLB Queen Ant** microservice orchestrates the aggregation (Crawler Ant) and analysis (Analytics Ant) microservices. This also performs other general housekeeping tasks.

### Inputs
1. Targeted Hitters List - text file with MLBids
2. Security Keys - Virtustream Object Store

### Execution
QA parses thorough the Targeted Hitters List and initiates a docker container to be run for each of the Hitters to be analyzed.  Security Keys to the Virtustream Object as well as the MLBids are passed to the docker container via environment variables.

### Outputs
No outputs...just docker kickers.

![](https://github.com/fire-ants/mlb-admin/blob/master/admin/mlb-pf-appflow-lg.png)
