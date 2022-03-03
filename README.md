
<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# ARA (Autonomous Robot for Autism)

ARA (Autonomous Robot for Autism)

## Summary

Husarion CORE2 - ROS w/Raspberry Pi 3 B+ & Ubuntu 16.04

Python 2.7


## How is it used?

# Installation Requirements

Install the following packages on the Husarion CORE2 - ROS board:

    #ROS Kinetick KEY update
    sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
    sudo apt-key del 421C365BD9FF1F717815A3895523BAEEB01FA116
    
    #update & upgrade packages, OpenCV will be installed with the ROS update
    sudo apt-get update && apt-get upgrade
    
    #install pip v19   
    curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"
    sudo python get-pip.py
    
    #install numpy requirements
    sudo apt-get install python-dev
    sudo apt install libatlas-base-dev
    
    #virtualenv system-wide install
    sudo pip install -U virtualenv
    
    #tensorflow virtualenv creation
    vitutalenv --system-site-packages -p python tensorflow
    
    #deploy tensorflow virtualenv
    source ~/tensorflow/bin/activate
    
    #install tensorflow
    pip install --upgrade pip
    sudo pip install 'https://github.com/lhelontra/tensorflow-on-arm/releases/download/v1.14.0-buster/tensorflow-1.14.0-cp27-none-linux_armv7l.whl'
    
    #install keras
    sudo pip install keras
    
    #deactivate tensorflow virtualenv
    deactivate

#Try
install tensorflow solving the swap problem
https://gist.github.com/EKami/9869ae6347f68c592c5b5cd181a3b205
problem solution with bazel
https://github.com/bazelbuild/bazel/commit/cc8e7166e29fee39d44e578cf98a06486084a6bd


## Data sources and AI methods
Random real face image files obtained from specific sources

## Challenges

FER

## What next?

Implementation


## Acknowledgments

DNA

# Setup

    cd ARA-3
    python ReconocerCara.py
 
