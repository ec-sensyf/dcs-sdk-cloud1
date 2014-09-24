## SenSyF SDK cloud2

### Description

This repository contains the first approach of the usecase to test the deployment on the operational cloud environment.

**IDEA**: Get Landsat 8 data from the catalogue, for a defined region, and crop small ROIs defined on kml files.
      The parallelization on this approach is performed by product (all ROIs are cropped on each task) on Hadoop.

**Usecase numbers**:

**Regions of interest ** - 3380 ROIs per task

--------------

### Instructions

1. Before enter on the sandbox run on your local machine:

      ```bash
      $ssh-add < username >.pem
      ```

2. Enter on the sandbox:

      ```bash
      $ ssh -A -i < username.pem > sensyf-sdk@< sandbox_host >
      ```

3. Run the following commands:

      ```bash
      cd
      git clone git@github.com:ec-sensyf/dcs-sdk-cloud1.git
      cd dcs-sdk-cloud1
      mvn install
      ```

--------------

Copyright (C) DEIMOS Engenharia S.A.
