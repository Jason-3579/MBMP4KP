# MBMP4KP Experimental Environment

## Hardware

- CPU: Intel Core i9-10900K
- Memory: 128 GB DDR4-3200
- GPU: NVIDIA GeForce RTX 2080 Ti
- GPU Memory: 11 GB
- GPU Compute Capability: 7.5

## Operating Environment

- Host OS: Windows 11
- Linux Environment: WSL2
- Linux Distribution: Ubuntu 22.04.5 LTS (Jammy Jellyfish)

## Development Environment

- VS Code: Windows host + WSL extension
- Project Path: `/home/wyl/MBMP4KP`
- Environment Manager: uv
- Virtual Environment: `.venv`

## Core Software Versions

- Python: 3.10.12
- uv: 0.12.5
- GCC: 11.4.0
- G++: 11.4.0
- GNU Make: 4.3
- NumPy: 1.26.4
- PyTorch: 2.5.1+cu121
- CUDA Runtime used by PyTorch: 12.1
- PyTorch Geometric: 2.6.1

## GPU Verification

PyTorch successfully detected the GPU:

- CUDA available: True
- GPU: NVIDIA GeForce RTX 2080 Ti
- GPU count: 1
- Compute capability: 7.5

A CUDA tensor matrix multiplication test completed successfully.

## PyTorch Geometric Verification

Both of the following layers successfully completed CUDA forward propagation:

- `GCNConv`
- `GATConv`

Therefore, the basic GPU graph-learning environment required by MBMP4KP has been verified.

## Reproducibility Policy

All formal MBMP4KP experiments will be conducted on this workstation and within this WSL2 environment.

Project dependencies are managed through:

- `pyproject.toml`
- `uv.lock`

Dependencies should be added through `uv` rather than installed manually with global `pip`.

The experimental software environment should remain fixed unless a dependency change is necessary for model implementation or baseline reproduction. Any such change must be documented.
