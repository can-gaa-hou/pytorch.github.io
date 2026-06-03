# Installing on ACC6 Platform
{:.no_toc}

ACC6 is a high-performance accelerator platform provided by Vendor6. This guide will help you install PyTorch with ACC6 support.

## Prerequisites
{: #acc6-prerequisites}

### Hardware Requirements

* ACC6-compatible accelerator hardware
* Supported operating system (Linux)

### Software Requirements

* Python 3.9-3.12
* ACC6 SDK or later

## Installation
{: #acc6-installation}

### pip

Use the pip package manager to install PyTorch with ACC6 support. Select your preferred options in the selector above to get the installation command.

## Verification
{: #acc6-verification}

To ensure that PyTorch was installed correctly with ACC6 support, run the following code:

```python
import torch
print(torch.__version__)

# Check ACC6 availability
if torch.backends.acc6.is_available():
    print("ACC6 is available!")
else:
    print("ACC6 is not available.")
```

## Documentation
{: #acc6-documentation}

For more information, please visit the [ACC6 Documentation](https://docs.vendor6.com/acc6).
