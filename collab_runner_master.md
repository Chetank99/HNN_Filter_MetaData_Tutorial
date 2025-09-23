If you are using a Google Colab notebook, you can use the below script to run the tutorial on your:
```
# Install hnn-core (dev version from master branch) in Google Colab

!git clone https://github.com/jonescompneurolab/hnn-core
%cd hnn-core
!pip install -e '.[dev]'
!python setup.py build_mod

# You are now good to GOOO!!!!
from hnn_core import jones_2009_model

# Create the default Jones 2009 model
net = jones_2009_model()
print(f"Network created with {len(net.cell_types)} cell types")
print(f"Cell types: {list(net.cell_types.keys())}")
```
