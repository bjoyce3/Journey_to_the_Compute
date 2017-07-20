# Day 2: Journey to the Compute


# Setting up the Hybrid workflow on Atmosphere and UA HPC

# Starting the master Atmosphere image
## Set password for the workflow
nano ~/.eemt-makeflow-password

Note: we'll use the password JourneytotheCompute

## Install Singularity
ezs

## Make a working directory
mkdir Desktop/singularityimages
cd Desktop/singularityimages/

## Clone the package from GitHub
git clone https://<github_username>@github.com/tyson-swetnam/sol-ot-comet-dev/
cd sol-ot-comet-dev/

## Run the master cloud image
./run-master examples/mcn_10m.tif 



# Starting an Atmosphere Worker

## Set up the same password file (with the same password!)
nano ~/.eemt-makeflow-password

ezs
git clone https://bjoyce3@github.com/tyson-swetnam/sol-ot-comet-dev
cd sol-ot-comet-dev/
./run-worker 

# Starting a University of Arizona High Performance Computing worker

## UA HPC specific setup
### Set up an xdisk space on the head node
xdisk -c create -m 50 -d 20

### Create a dir for the images
cd /xdisk/<username>/
mkdir singularityimages

### Request a node 
qsub -I -N <username>_singularity_worker -m bea -M <useremail>.arizona.edu -W group_list=<usergroupatUAHPC> -q windfall -l select=1:ncpus=1:mem=8gb -l cput=1:0:0 -l walltime=1:0:0

### Bring up Singularity and change to the bash setting
module load singularity
bash

### Set the PATH variable on the HPC node
singularity shell eemt-current.img
export PATH=/opt/eemt/bin:/opt/eemt/grass-7.2.0/bin:$PATH

## Now you're on the node, here's what to do

### Set up the project

cd /xdisk/<username>/singularityimages
wget http://xd-login.opensciencegrid.org/scratch/eemt/singularity/eemt-current.img

### 