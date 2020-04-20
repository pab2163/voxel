Bootstrap:docker
From:ubuntu:latest

%post
apt-get update

apt-get install -y r-base-core
R --slave -e 'install.packages("voxel")'
