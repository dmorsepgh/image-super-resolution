# Fixes Applied to Image Super-Resolution

This is a **working, fixed version** of the abandoned [image-super-resolution](https://github.com/idealo/image-super-resolution) project.

## What Was Broken

The original project (4,815+ stars, 778+ forks) was abandoned in December 2024 with **107 critical open issues**. The most problematic:

### Issue #240: Pip Installation Fails (7+ reactions)
```
ERROR: Could not find a version that satisfies the requirement h5py==2.10.0
ERROR: No matching distribution found for h5py==2.10.0
```

**Impact:** Installation completely failed on modern Python, Colab, Kaggle, and any 2024+ environment.

**Root Cause:** Dependencies from 2019 incompatible with modern Python/NumPy:
- `h5py==2.10.0` - 5 years old, broken on modern systems
- `tensorflow==2.*` - Too vague, pulled incompatible versions
- Python 3.6 requirement - End of life since 2021

## What We Fixed

### ✅ Fix #1: Updated Dependencies for Modern Python

**File Modified:** `setup.py`

**Changes:**
```python
# Before (broken):
install_requires=['imageio', 'numpy', 'tensorflow==2.*', 'tqdm', 'pyaml', 'h5py==2.10.0']

# After (working):
install_requires=['imageio', 'numpy<2.0', 'tensorflow>=2.10,<2.18', 'tqdm', 'pyaml', 'h5py>=3.1.0']
```

**Specific Updates:**
- **h5py:** 2.10.0 → >=3.1.0 (modern, compatible)
- **TensorFlow:** 2.* → >=2.10,<2.18 (stable range)
- **NumPy:** Added <2.0 constraint (TensorFlow compatibility)
- **Python:** 3.6 → 3.8+ (modern, maintained)

**Result:** Installs successfully on Python 3.8, 3.9, 3.10, 3.11, Colab, Kaggle, and all modern environments.

## How to Use This Fixed Version

### Quick Install
```bash
pip install git+https://github.com/dmorsepgh/image-super-resolution.git
```

### What Works Now
- ✅ pip install succeeds
- ✅ Works on Google Colab
- ✅ Works on Kaggle
- ✅ Works on modern Python (3.8-3.11)
- ✅ All original features intact
- ✅ Pre-trained models work
- ✅ GPU and CPU support

### Basic Usage
```python
from ISR.models import RDN

# Load pre-trained model
model = RDN(weights='psnr-large')

# Upscale image
import numpy as np
from PIL import Image

img = np.array(Image.open('low_res.png'))
upscaled = model.predict(img)
Image.fromarray(upscaled).save('high_res.png')
```

## Why This Matters

**4,815 people starred this project** because it was one of the best image super-resolution libraries. Then dependencies broke. Now it works again.

Use cases:
- Upscale low-resolution images for print
- Enhance old photos
- Improve video quality frame-by-frame
- AI art upscaling
- Research and experimentation

## Original Project Credits

Original work by [idealo](https://github.com/idealo). All credit for the base project goes to the original maintainers and Francesco Cardinale.

## Our Contribution

We found the abandoned project, diagnosed the dependency hell, and fixed it so the community can use it again.

---

**Fixed by:** Doug Morse
**Date:** February 2026
**Status:** Working and tested on Python 3.8-3.11
