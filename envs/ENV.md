# Szybki start (Conda):

'''{powershel}
conda env create -f envs/environment-datascience.yml
conda env create -f envs/environment-datascience-dl.yml
conda env create -f envs/environment-datascience-geo.yml
'''
# Rejestracja kernelów Jupyter:

conda activate DataScience
python -m pip install ipykernel
python -m ipykernel install --user --name DataScience --display-name "Python (DataScience)"

conda activate DataScience_DL
python -m pip install ipykernel
python -m ipykernel install --user --name DataScience_DL --display-name "Python (DataScience_DL)"

conda activate DataScience_Geo
python -m pip install ipykernel
python -m ipykernel install --user --name DataScience_Geo --display-name "Python (DataScience_Geo)"

# PyTorch GPU (opcjonalnie):
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124