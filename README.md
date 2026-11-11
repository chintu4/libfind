# libfind

A Python utility to help developers quickly locate functions and classes in large packages and libraries.

## Installation

Install via pip:

```bash
pip install libfind
```

Or using `uv`:

```bash
uv pip install libfind
```

In Google Colab or Kaggle:

```python
!pip install libfind
```

Or install directly from GitHub:

```bash
pip install git+https://github.com/chintu4/libfind.git
```

## Quick Start

### Example: Locate where a function is defined
Find where `train_test_split` is located inside `sklearn`:

```python
import libfind

result = libfind.find_function("sklearn", "train_test_split")
print(result)
```

**Output:**

```python
{
    'package': 'sklearn',
    'function': 'train_test_split',
    'module': 'sklearn.model_selection._split',
    'file': '/usr/local/lib/python3.12/dist-packages/sklearn/model_selection/_split.py',
    'line': 2752
}
```

## Contributing

Feel free to open an issue or submit pull requests for suggestions, improvements, or new features!
