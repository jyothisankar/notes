sudo apt-get install -y podman 

sudo apt-get install -y git git-lfs


mkdir sankar

cd sankar

git clone git@github.ibm.com:IBM-Z-Feature-Appliance-Base/zFAB-Source.git

git clone git@github.ibm.com:IBM-Z-Feature-Appliance-Base/zFAB-Werkbank.git

git clone git@github.ibm.com:IBM-Z-Feature-Appliance-Base/zFAB-Extensions.git

git clone git@github.ibm.com:IBM-Z-Feature-Appliance-Base/zaci_cicd_buildimage.git

sudo podman login docker.io



