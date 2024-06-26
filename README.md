[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)

# Gamba
Implementation of "GAMBA: MARRY GAUSSIAN SPLATTING WITH MAMBA FOR SINGLE-VIEW 3D RECONSTRUCTION" in PyToch.

![Diagram](diagram.png)

## install
`$ pip install gamba-torch`

## usage
```python
import torch 
from gamba.main import Gamba


# Forward pass of the GambaDecoder module.
x = torch.randn(1, 1000, 512)

# Model
model = Gamba(
    dim=512,
    d_state=512,
    d_conv=512,
    n=16384,
    depth=3
)

# Out
out = model(x)
print(out)
```


# License
MIT

# Todo
- [ ] Paper Link
- [ ] Citation bibtex