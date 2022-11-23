## Let's assume we have downloaded the random survival forest (RSF) models at the following location 

github: https://github.com/aesc1217/RSF_DFSP

/Users/xxx/Desktop/rsf_model_T2W.zip  # RSF model based on radiomics features derived from T2W images

/Users/xxx/Desktop/rsf_model_T1WC.zip # RSF model based on radiomics features derived from T1WC images

/Users/xxx/Desktop/rsf_model_T1WC_T2W.zip # RSF model based on radiomics features derived from both T1WC and T2W images

## Install PySurvival 

https://square.github.io/pysurvival/installation.html

## Code sample (Loading RSF model)


```python
from pysurvival.utils import load_model

# Load RSF model based on radiomics features derived from T2W images
rsf_model_T2W = load_model('/Users/xxx/Desktop/rsf_model_T2W.zip')

# Load RSF model based on radiomics features derived from T1WC images
rsf_model_T1WC = load_model('/Users/xxx/Desktop/rsf_model_T1WC.zip')

# Load RSF model based on radiomics features derived from both T1WC and T2W images
rsf_model_T1WC = load_model('/Users/xxx/Desktop/rsf_model_T1WC_T2W.zip')

```
