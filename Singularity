Bootstrap:docker
From:ubuntu:latest


# Installations
%post
apt-get update

apt-get install -y r-base-core
R --slave -e 'install.packages("voxel")'

# Test load package
%runscript
#!/bin/bash
Rscript --slave "test_load_voxel_package.R"
