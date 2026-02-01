# Image Super-Resolution - Fixed & Working (AI Upscaling Library)

**Upscale Images 4X With AI. No Monthly Fees. Works Offline.**

The most popular AI image upscaling library on GitHub (4,800+ stars) broke in 2024. This is the fixed version that actually works.

---

## The Problem

You need to upscale images. You found the perfect AI library. You tried to install it.

💥 **Installation failed.**

```
ERROR: Could not find a version that satisfies the requirement h5py==2.10.0
pip install failed
```

You tried:
- Different Python versions
- Virtual environments
- Stack Overflow solutions
- GitHub issues (107 open, no fixes)

**Nothing worked.** The project was abandoned.

So you either:
- Paid for online AI upscaling ($10-30/month)
- Used lower-quality tools
- Gave up on AI upscaling

---

## The Solution

We fixed it.

Diagnosed the dependency hell. Updated to modern Python. Tested on Colab, Kaggle, and local environments.

**It works now.**

One command. Upscale any image 4X with AI. Run locally. No monthly fees.

---

## What You Get

✅ **Working AI upscaling library** - Installs successfully, runs perfectly
✅ **Pre-trained models** - Ready to use, no training required
✅ **4X upscaling** - 512px → 2048px with AI enhancement
✅ **Multiple models** - RDN, RRDN optimized for different use cases
✅ **GPU & CPU support** - Works with or without NVIDIA GPU
✅ **Colab/Kaggle compatible** - Works in notebooks
✅ **Full documentation** - What was broken, how we fixed it, how to use it
✅ **GitHub repo access** - Fork it, modify it, use commercially

---

## What It Does

**AI Image Super-Resolution:**
- Upscale low-res images 2X or 4X
- Enhance details with AI (not just interpolation)
- Restore old/degraded photos
- Prepare images for print
- Video frame enhancement
- AI art upscaling

**Powered by:**
- Residual Dense Networks (RDN)
- Residual in Residual Dense Network (RRDN)
- Pre-trained on ImageNet
- PSNR and GAN-based models

---

## Who This Is For

✅ Photographers enhancing old photos
✅ Print shops needing high-res from low-res
✅ AI artists upscaling generated images
✅ Researchers running experiments
✅ Developers building image enhancement apps
✅ Anyone who needs offline AI upscaling
✅ People tired of $10-30/month subscriptions

---

## Requirements

- Python 3.8+ (works on 3.8, 3.9, 3.10, 3.11)
- 4GB+ RAM (8GB+ recommended)
- Optional: NVIDIA GPU with CUDA (faster, but works on CPU)
- Works on: Mac, Windows, Linux, Colab, Kaggle

---

## Why This Works When the Original Doesn't

**The Problem:** The original used 5-year-old dependencies incompatible with modern Python:
- `h5py 2.10.0` (2019) - Broken on modern NumPy
- `tensorflow 2.*` - Too vague, pulled incompatible versions
- Python 3.6 requirement - End of life since 2021

**The Fix:** Updated to modern, stable versions:
- `h5py >=3.1.0` - Compatible with modern systems
- `tensorflow >=2.10,<2.18` - Stable, tested range
- `numpy <2.0` - TensorFlow compatibility
- Python 3.8+ - Modern, maintained

**The Result:** Works on Colab, Kaggle, modern Python, everywhere.

---

## Usage Example

```python
# Install (one command)
pip install git+https://github.com/dmorsepgh/image-super-resolution.git

# Use (three lines)
from ISR.models import RDN
model = RDN(weights='psnr-large')
upscaled_img = model.predict(your_low_res_image)
```

That's it. Your image is now 4X larger with AI-enhanced details.

---

## Compare Your Options

| Option | Cost | Quality | Privacy | Speed |
|--------|------|---------|---------|-------|
| **Online AI upscaler (Topaz, etc.)** | $10-30/month | High | Uploads to cloud | Fast |
| **Free online tools** | Free | Low-Medium | Public upload | Slow |
| **Original broken library** | Free | N/A | N/A | Doesn't work |
| **This fixed version** | $27 once | High | Local only | GPU: Fast / CPU: Medium |

**Your images stay on your machine. No uploads. No monthly fees.**

---

## Pricing

**$27** - One-time payment

**What you save:**
- $10-30/month in subscription fees (saves $120-360/year)
- Hours debugging the broken original
- Privacy (no cloud uploads)

**ROI:** Pays for itself in 1 month vs subscriptions.

---

## What's Included

📦 **Fixed codebase** - Works on modern Python
📦 **Pre-trained models** - RDN, RRDN ready to use
📦 **Documentation** - Installation, usage, examples
📦 **Technical breakdown** - What was broken, how we fixed it
📦 **GitHub repo access** - Fork, modify, use commercially
📦 **Free updates** - Any future fixes included

---

## Guarantee

**If pip install doesn't work, full refund.** No questions asked.

We tested this on Python 3.8-3.11, Colab, Kaggle, Mac, and Linux. It works.

---

## Use Cases

### Photography
- Restore old family photos
- Enhance low-res scans
- Prepare images for large prints

### AI Art
- Upscale Stable Diffusion/Midjourney outputs
- Enhance details in generated images
- Create high-res versions for print

### Video
- Upscale video frames
- Enhance old footage
- Improve streaming quality

### Development
- Build image enhancement apps
- Integrate into workflows
- Research and experiments

---

## FAQ

**Q: Is this legal?**
A: Yes. The original is open source (Apache 2.0). This is a fixed fork with proper attribution.

**Q: Do I need a GPU?**
A: No. Works on CPU (slower) or GPU (faster). Any modern computer works.

**Q: How does this compare to Topaz AI?**
A: Similar quality, but offline and no subscription. Topaz has more features, this has no monthly fee.

**Q: Will this work on my Mac M1/M2?**
A: Yes. CPU mode works great on Apple Silicon.

**Q: What about GIMP/Photoshop upscaling?**
A: Those use interpolation. This uses AI trained on millions of images. Much better quality.

**Q: Can I use this commercially?**
A: Yes. Use it for client work, products, whatever you want.

**Q: What if I get stuck?**
A: Email support included. I'll help you get it working.

---

## About Me

I'm Doug Morse. I find valuable abandoned open source projects, fix them, and redistribute them.

**4,815 people** starred this AI upscaling library because it was one of the best. Then it broke. I fixed it.

---

## Get Started Now

**$27 - One-time payment**

Download immediately after purchase:
- Complete fixed codebase
- Pre-trained AI models
- Full documentation
- GitHub access
- Email support

**Stop paying monthly. Start upscaling locally.**

[Buy Now]

---

## Fine Print

- One-time payment, yours forever
- No subscription, no recurring fees
- 30-day money-back guarantee
- Use personally or commercially
- Free updates included
- Support: doug@dmpgh.com

---

**Questions?** Email: doug@dmpgh.com

**License:** Apache 2.0 (same as original)
