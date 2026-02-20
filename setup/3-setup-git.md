# 1. Navigate to your Documents folder and create the project folder
mkdir -p ~/Documents/data-analysis && cd ~/Documents/data-analysis

# 2. Create a virtual environment
python -m venv env

# 3. Activate the environment
# Windows:
if [ "$(uname -s | grep -i cygwin || uname -s | grep -i mingw)" ]; then
    env\Scripts\activate
# macOS/Linux:
else
    source env/bin/activate
fi

# 4. Upgrade pip and install tools
python -m pip install --upgrade pip
python -m pip install jupyter pandas numpy matplotlib seaborn scipy scikit-learn

# 5. Launch Jupyter Notebook
jupyter notebook


# Notes:
# Windows: Activate with
#   env\Scripts\activate
# macOS/Linux: Activate with
#   source env/bin/activate