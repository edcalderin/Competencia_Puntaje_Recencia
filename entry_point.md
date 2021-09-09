Command: `conda create --name keyboard_paper_competition_env`
which would
- Create a new virtual environment for this project

Command: `start vs_BuildTools.exe`
which would
- It is a file downloaded from https://visualstudio.microsoft.com/es/visual-cpp-build-tools/. It must be installed before executing the next step.
- Only check "C++ Build tools" and then Install. It will take some minutes.
- Restart is required.

Command: `pip install -r requirements.txt`
which would
- Create a new virtual environment for this project

Command: `unzip data/raw/data.zip -d data/raw/`  
which would
- Unzip original datasets in the current folder

Command: `unzip data/processed/data_processed.zip -d data/processed/`  
which would
- Unzip processed datasets in the current folder, it is useful if do not want waste time processing data and go forward to training