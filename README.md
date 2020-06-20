# efficientnet-lite0-pytorch-model

Pretrained Pytorch model file for EfficientNet Lite0

## Installation

```
pip install efficientnet_lite0_pytorch_model
```


## Basic Usage

```
from efficientnet_lite0_pytorch_model import EfficientnetLite0ModelFile
print( 'model file path is %s' % ( EfficientnetLite0ModelFile.get_model_file_path() ) )
```

## Actual Usage

Install the model package from [EfficientNet-Lite-PyTorch](https://github.com/ml-illustrated/EfficientNet-Lite-PyTorch):
```
pip install efficientnet_lite_pytorch
```

Load the model with pretrained weights:
```
from efficientnet_lite_pytorch import EfficientNet

from efficientnet_lite0_pytorch_model import EfficientnetLite0ModelFile
weights_path = EfficientnetLite0ModelFile.get_model_file_path()

lite0_model = EfficientNet.from_pretrained('efficientnet-lite0', weights_path = weights_path )
```

## Credits

This package was created with _Cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.

- _Cookiecutter: https://github.com/audreyr/cookiecutter
- _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
