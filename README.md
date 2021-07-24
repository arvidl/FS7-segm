# FreeSurfer 7.x hints and scripts



## MacOS (July 2021)


### Install and Setup 7.2.0 for MacOS: see [here](https://surfer.nmr.mgh.harvard.edu/fswiki//FS7_mac)


- freesurfer-darwin-macOS-7.2.0.pkg 
- XQuartz-2.8.1.dmg


Uninstall 7.1.1:
```bash
sudo cp -r /Applications/freesurfer/7.1.1/MCRv84 /Applications/freesurfer/7.2.0/
sudo cp /Applications/freesurfer/7.1.1/license.txt /Applications/freesurfer/7.2.0/

sudo bash /Applications/freesurfer/7.1.1/uninstall.sh 

# This could be added to ~./.zshrc or run interactively:
export FREESURFER_HOME=/Applications/freesurfer/7.2.0
export SUBJECTS_DIR=$FREESURFER_HOME/subjects
source $FREESURFER_HOME/SetUpFreeSurfer.sh
```


