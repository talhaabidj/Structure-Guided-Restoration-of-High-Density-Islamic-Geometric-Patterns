# Structure-Guided Restoration of High-Density Islamic Geometric Patterns

[![License: CC BY-NC 4.0](https://img.shields.io/badge/Docs-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![License: GPL v3](https://img.shields.io/badge/Code-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

> **Research Status:** 🔬 In Progress | Ground Level Phase

## Abstract

This research investigates the application of **structure-guided deep learning methods** for restoring damaged Islamic geometric patterns in heritage sites. We address a critical gap: existing inpainting models fail on "High-Density" patterns (Edge Density > 40%) because they treat geometry as texture.

**Our Hypothesis:** Structure-first approaches (like EdgeConnect) outperform global-context approaches (like LaMa) for preserving geometric fidelity in complex patterns.

## The Research Gap

| What Exists | What's Missing |
|-------------|----------------|
| 3D scanning of heritage sites | Deep learning **restoration** of 2D patterns |
| GAN-based pattern **generation** | Benchmarks for **High-Density** (>40% edge density) |
| General inpainting (faces, landscapes) | Domain-specific evaluation for geometric accuracy |

## Repository Structure

```
Research_Paper/
├── docs/
│   ├── Research_Context.md   # Master plan & methodology
│   ├── Literature_Review.md  # Annotated bibliography
│   └── Gap_Analysis.md       # Detailed research gaps
├── dataset/                   # Islamic Patterns Dataset (4,000+ images)
├── notebooks/                 # Training notebooks (coming soon)
├── scripts/                   # Utility scripts (coming soon)
└── LICENSE                    # CC BY-NC 4.0 (docs) + GPLv3 (code)
```

## Key Documents

| Document | Description |
|----------|-------------|
| [Research Context](docs/Research_Context.md) | Full methodology, scope definition, and roadmap |
| [Literature Review](docs/Literature_Review.md) | Survey of inpainting methods and evaluation metrics |
| [Gap Analysis](docs/Gap_Analysis.md) | Detailed breakdown of 6 identified research gaps |

## Methodology

1. **Restoration vs. Recreation:** We use simulated damage on known ground-truth images to validate accuracy (PSNR/SSIM).
2. **Models Compared:** OpenCV (baseline), EdgeConnect (structure-guided), LaMa (global context).
3. **Data Augmentation:** Online 8x expansion via rotations and flips (valid for symmetric patterns).

## Preliminary Results

| Model | PSNR (dB) | SSIM | Notes |
|-------|-----------|------|-------|
| OpenCV Telea | 21.27 | 0.72 | Classical baseline |
| LaMa | 23.59 | 0.83 | Higher pixel accuracy |
| EdgeConnect | 23.36 | **0.88** | Higher structural accuracy ★ |

## License

- **Documentation:** [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) — Share with attribution, no commercial use.
- **Code:** [GPLv3](https://www.gnu.org/licenses/gpl-3.0) — Open source, copyleft.

## Citation

If you use this work, please cite:

```bibtex
@misc{abid2025islamic,
  author = {Talha Abid},
  title = {Structure-Guided Restoration of High-Density Islamic Geometric Patterns},
  year = {2025},
  publisher = {GitHub},
  url = {https://github.com/YOUR_USERNAME/YOUR_REPO}
}
```

## Author

**Talha Abid**

---

*This research is ongoing. Contributions and feedback are welcome via Issues.*
