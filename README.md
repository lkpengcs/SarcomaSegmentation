# Performance of deep learning-based segmentation of soft tissue sarcoma by MRI sequence, tumor type and location

This repository provides the trained weights and usage guide for the segmentation model described in our [paper](https://link.springer.com/article/10.1007/s00256-026-05178-3).


### Implementation
Our model is built and trained using the **[nnU-Net v1](https://github.com/MIC-DKFZ/nnUNet/tree/nnunetv1)** framework. 

To use our model, please:
1. Install the official `nnunet` (v1) library.
2. Follow the standard [nnU-Net directory structure](https://github.com/MIC-DKFZ/nnUNet/blob/nnunetv1/documentation/setting_up_paths.md) for environment variables.

---

### Pretrained Model Weights
The best-performing 3D full-resolution model weights are available here:

* **Google Drive:** [Download Weights](https://drive.google.com/drive/folders/1kNFw58U7bW2xtppp_gOslcX-8RGcUuH-?usp=sharing)

**Usage:**
Place the downloaded folder into your `$RESULTS_FOLDER/nnUNet/3d_fullres/` directory. You can then run inference using:
```bash
nnUNet_predict -i INPUT_FOLDER -o OUTPUT_FOLDER -t TaskXXX_XXX -m 3d_fullres
```


### Citation

If you find this work useful in your research, please consider citing:

```bibtex
@article{peng2026performance,
  title={Performance of deep learning-based segmentation of soft tissue sarcoma by MRI sequence, tumor type and location},
  author={Peng, Linkai and Perronne, Laetitia and Gennaro, Nicol{\`o} and Rashidi, Ahmad Pour and Kobus, Zuzanna and Seo, Mirinae and Borhani, Amir A and Kelahan, Linda and Subedi, Kamal and Savas, Hatice and others},
  journal={Skeletal Radiology},
  pages={1--10},
  year={2026},
  publisher={Springer}
}
