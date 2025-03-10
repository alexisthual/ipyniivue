# ipyNiiVue
Try out in mybinder: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/niivue/ipyniivue/HEAD)       
display and interact with a NIfTI image in a WebGl 2.0 canvas within a Jupyter notebook cell

## Installation
```sh
git clone https://github.com/niivue/ipyniivue
cd ipyniivue
yarn
yarn run build
pip install -e .
```
```
jupyter lab
```

## Usage
example usage
```py
from ipyniivue import Niivue

nv = Niivue(logging=True)
volumes = [
    {
        'url': 'https://niivue.github.io/niivue/images/mni152.nii.gz',
        'opacity': 1,
        'visible': True,
    }
]
nv.load_volumes(volumes)
nv
```
![example](docs/example.png)
