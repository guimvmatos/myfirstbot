install anaconda

install Microsoft Visual C++ Redistributable

create a folder for our project (myfirstbot)

cmd.exe
cd + path for our folder
conda create --name chatbotvenv python==3.7.6
conda activate chatbotvenv
conda install ujson==2.0.3
conda install tensorflow==2.1.0
pip install rasa==1.10.0
rasa init