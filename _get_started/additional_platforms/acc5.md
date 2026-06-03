# Installing on ACC5 Platform
{:.no_toc}

ACC5 is a high-performance accelerator platform provided by Vendor5. This guide will help you install PyTorch with ACC5 support.

## Prerequisites
{: #acc5-prerequisites}

### Hardware Requirements

* ACC5-compatible accelerator hardware
* Supported operating system (Linux)

### Software Requirements

* Python 3.9-3.12
* ACC5 SDK or later

## Installation
{: #acc5-installation}

### pip

Use the pip package manager to install PyTorch with ACC5 support. Select your preferred options in the selector above to get the installation command.

## Verification
{: #acc5-verification}

To ensure that PyTorch was installed correctly with ACC5 support, run the following code:

```python
import torch
print(torch.__version__)

# Check ACC5 availability
if torch.backends.acc5.is_available():
    print("ACC5 is available!")
else:
    print("ACC5 is not available.")
```

## Documentation
{: #acc5-documentation}

For more information, please visit the [ACC5 Documentation](https://docs.vendor5.com/acc5).
