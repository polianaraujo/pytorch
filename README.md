# Learning Pytorch
This repository will contain my PyTorch learnings for Deep Learning with Datacamp.

## Introdução ao Aprendizado Profundo com PyTorch

### Tensors: the building blocks of netoworks in PyTorch

- Load from list
``` python
import torch
lst = [ [1,2,3] , [4,5,6] ]
tensor = torch.tensor(lst)
```

- Loaf from NumPy array
``` python
np_array = np.array(array)
np_tensor = torch.from_numpy(nop_array)
```

## How to create the first neural network

As redes neurais são entradas empilhadas, camadas ocultas e saídas.

Começamos construindo uma rede básica de duas camadas, sem camadas ocultas.
