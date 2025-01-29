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

## How to execute a step forward

### Binary classification: forward pass

``` python
# Create input data of shape 5x6
input_data = torch.tensor(
    [[-0.4421, 1.5207, 2.0607, -0.3647, 0.4691, 0.0946],
    [-0.9155, -0.0475, -1.3645, 0.6336, -1.9520, -0.3398],
    [0.7406, 1.6763, -0.8511, 0.2432, 0.1123, -0.0633],
    [-1.6630, -0.0718, -0.1285, 0.5396, -0.0288, -0.8622],
    [-0.7413, 1.7920, -0.0883, -0.6685, 0.4745, -0.4245]])

# Create binary classification model
model = nn.Sequential(
    nn.Linear(6,4) # First Linear layer
    nn.Linear(4,1) # First Linear layer
    nn.Sigmoid()   # Sigmoid activation function
)

# Pass input data through model
output = model(input_data)
```