#[DRAFT]

### Overview
We propose a flexible conditional modeling framework that learns structured dependencies between variables by blending linear and nonlinear transformations. Our method dynamically adjusts to data characteristics via a learnable mixture parameter, allowing the model to preserve simplicity where appropriate while capturing complex behaviors when necessary. We validate the approach on synthetic nonlinear datasets, achieving significant improvements over traditional linear models. This framework opens the door for scalable integration into large models, including language model retraining where structured paths in latent space matter.

## Features
- Dynamic alpha-weighted mixture of linear and nonlinear paths
- Experiments on:
  - Simple synthetic functions
  - Spiral curve datasets
  - OpenMathReasoning (real-world text embeddings)
- Full paper included

### Usage
``` python
from kln import FlexibleConditional

model = FlexibleConditional(input_dim=2, hidden_dim=64, output_dim=1)
```

### Acknowledgements
OpenAI's ChatGPT provided substantial assistance with the research, writing, and development of this work. The authors gratefully acknowledge its contributions while assuming full responsibility for the final content.

We thank the contributors to open-source geometry libraries and acknowledge the support of interdisciplinary visualization research.
