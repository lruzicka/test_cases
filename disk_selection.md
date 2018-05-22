# Disk Selection

## Release criteria

The given criteria must be completely fulfilled, otherwise the test must be considered a fail. In such case, file a bug and describe the misbehaviour as thoroughly as possible. Also, propose the bug as a Beta blocker.

* Users must be able to select to which of the disks, connected to the system, Fedora will be installed.
* Other disks must not be affected anyhow by the installation process. 

## How to test

1. Use a bare metal computer with two disks or prepare a VM set-up with two virtual disks.
2. Use any Fedora image to start the installation. If you are using the Live Image, boot into the live system and choose **Install to Hard Drive**.
3. In Anaconda, click on **Installation Destination** to choose the target disk.
4. Select one of the disks. There should be at least 12GB of free space available to make sure the installer will be able to operate properly. For a Live image, 10GB is sufficient.
5. Unless you want to test for advanced disk partitioning functions, use the automatic **Storage Configuration**. 
6. Install the system.
7. Boot into the freshly installed system.


## Test evaluation

The test passes if:

* no error is reported during the installation
* the system boots without any user intervention
* the second disk (the one not selected for the installation) is in its previous state




