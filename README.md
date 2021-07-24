# FreeSurfer 7.x hints and scripts



## MacOS (July 2021)
[ReleaseNotes](https://surfer.nmr.mgh.harvard.edu/fswiki/ReleaseNotes)

### Install and Setup 7.2.0 for MacOS
See [here](https://surfer.nmr.mgh.harvard.edu/fswiki//FS7_mac)

- [rel7downloads](https://surfer.nmr.mgh.harvard.edu/fswiki/rel7downloads)  or [here](https://surfer.nmr.mgh.harvard.edu/pub/dist/freesurfer/7.2.0) `freesurfer-darwin-macOS-7.2.0.pkg`  $\mapsto$  --- freesurfer-darwin-macOS-7.2.0-20210713-aa8f76b ---
- XQuartz-2.8.1.dmg


Substitute FS 7.1.1 with 7.2.0:
```bash
sudo cp -r /Applications/freesurfer/7.1.1/MCRv84 /Applications/freesurfer/7.2.0/
sudo cp /Applications/freesurfer/7.1.1/license.txt /Applications/freesurfer/7.2.0/

sudo bash /Applications/freesurfer/7.1.1/uninstall.sh 

# This could be added to ~./.zshrc or run interactively:
export FREESURFER_HOME=/Applications/freesurfer/7.2.0
export SUBJECTS_DIR=$FREESURFER_HOME/subjects
source $FREESURFER_HOME/SetUpFreeSurfer.sh

# Test freeview (v. 3.0)
freeview /Applications/freesurfer/7.2.0/subjects/bert/mri/brain.mgz
```


