# Szybki start (Conda):

```powershell
conda env create -f envs/environment-datascience.yml
conda env create -f envs/environment-datascience-dl.yml
conda env create -f envs/environment-datascience-geo.yml
```
# Rejestracja kernelów Jupyter:

```powershell
conda activate DataScience
python -m pip install ipykernel
python -m ipykernel install --user --name DataScience --display-name "Python (DataScience)"
```
```powershell
conda activate DataScience_DL
python -m pip install ipykernel
python -m ipykernel install --user --name DataScience_DL --display-name "Python (DataScience_DL)"
```
```powershell
conda activate DataScience_Geo
python -m pip install ipykernel
python -m ipykernel install --user --name DataScience_Geo --display-name "Python (DataScience_Geo)"
```
# PyTorch GPU (opcjonalnie):
```powershell
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
```