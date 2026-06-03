# Installing on ACC4 Platform
{:.no_toc}

ACC4 is a high-performance accelerator platform provided by Vendor4. This guide will help you install PyTorch with ACC4 support.

## Prerequisites
{: #acc4-prerequisites}

### Hardware Requirements

* ACC4-compatible accelerator hardware
* Supported operating system (Linux)

### Software Requirements

* Python 3.9-3.12
* ACC4 SDK or later

## Installation
{: #acc4-installation}

### pip

Use the pip package manager to install PyTorch with ACC4 support. Select your preferred options in the selector above to get the installation command.

## Verification
{: #acc4-verification}

To ensure that PyTorch was installed correctly with ACC4 support, run the following code:

```python
import torch
print(torch.__version__)

# Check ACC4 availability
if torch.backends.acc4.is_available():
    print("ACC4 is available!")
else:
    print("ACC4 is not available.")
```

## Documentation
{: #acc4-documentation}

For more information, please visit the [ACC4 Documentation](https://docs.vendor4.com/acc4).
