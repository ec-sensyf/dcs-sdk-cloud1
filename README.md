dcs-sdk-cloud1
==============

DESCRIPTION

This repository contains the first approach of the usecase to test the deployment on the operational cloud environment.

IDEA: Get Landsat 8 data from the catalogue, for a defined region, and crop small ROIs defined on kml files.
      The parallelization on this approach is performed by product (all ROIs are cropped on each task) on Hadoop.

Usecase numbers:

Regions of interest (ROIs) - 3380

--------------

INSTRUCTIONS
1. Before enter on the sandbox run on your local machine:

      $ssh-add < username >.pem
      
2. Enter on the sandbox:

      $ ssh -A -i < username.pem > sensyf-sdk@< sandbox_host >
      
3. Run the following commands:

      $ cd

      $ git clone git@github.com:ec-sensyf/dcs-sdk-cloud1.git
      
      $ cd dcs-sdk-cloud1
      
      $ mvn install

--------------

Copyright (C) DEIMOS Engenharia S.A.
