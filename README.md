# Sparse-View Ultra-Low-Dose CT Reconstruction via Med-NeRF

An implicit neural representation framework (Med-NeRF) in PyTorch that reconstructs 2D/3D organ density volumes from ultra-sparse X-ray projections (4 to 16 views) under Poisson photon noise, eliminating classical Filtered Backprojection (FBP) streak artifacts.

## Key Results
Evaluated across sparse projection angles under physical Poisson noise:
- **N = 4 Views:** Med-NeRF achieves **11.91 dB PSNR / 0.3583 SSIM** vs FBP's **9.62 dB PSNR / 0.2454 SSIM** (**+2.29 dB Gain**).
- **N = 8 Views:** Med-NeRF achieves **13.74 dB PSNR / 0.4331 SSIM** (**+1.41 dB Gain**).
- **N = 16 Views:** Med-NeRF achieves superior structural fidelity with an **SSIM of 0.5370** vs FBP's **0.4211**.

## Repository Contents
- `med_nerf_sparse_ct.ipynb`: Complete PyTorch pipeline for phantom generation, Poisson noise simulation, ray marching, and evaluation.
- `Sparse_CT_Med_NeRF.pdf`: IEEE-formatted multi-column manuscript draft.

## Author
- **Ashutosh Mishra** — B.Tech ECE, Netaji Subhas University of Technology (NSUT), New Delhi
