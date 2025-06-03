
<!-- <div align= "center">
    <h1> Official repo for Sparse-vDiT</h1>

</div> -->

<h3 align="center"><strong>Sparse-vDiT: Unleashing the Power of Sparse Attention to Accelerate Video Diffusion Transformers</strong></h3>


<div align="center">
<a href='https://arxiv.org/abs/2504.06263'><img src='https://img.shields.io/badge/arXiv-2504.06263-b31b1b.svg'></a> &nbsp;&nbsp;&nbsp;&nbsp;
 <a href='https://omnisvg.github.io/'><img src='https://img.shields.io/badge/Project-Page-Green'></a> &nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://huggingface.co/OmniSVG"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Weights-HF-orange"></a> &nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://huggingface.co/OmniSVG"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Dataset%20-HF-orange"></a>
</div>

## 🔥🔥🔥 News !!

- [2025/04/09] 👋 Release MMSVG-Icon and MMSVG-Illustration 🤗[Dataset](https://huggingface.co/OmniSVG).
- [2025/04/09] 👋 Upload paper and init project. [Read](https://arxiv.org/abs/2504.06263)
<p align="center">
    <img src="assets/OmniSVG-demo-gen-proc-anime-1080.gif" alt="Demo GIF" width="720px" />
</p>


## To Do List
- [ ] Code and Pretrained Models Release 
- [ ] MMSVG-Character Dataset Release
- [x] MMSVG-Icon and MMSVG-Illustration Dataset Release
- [x] Project Page & Technical Report


## 🏃 Introduction

**OmniSVG** is the first family of end-to-end multimodal SVG generators that leverage pre-trained Vision-Language Models (VLMs), capable of generating complex and detailed SVGs, from simple icons to intricate anime characters. By parameterizing SVG commands and coordinates into discrete tokens, OmniSVG decouples structural logic from low-level geometry for efficient training while maintaining the expressiveness of complex SVG structure. To further advance the development of SVG synthesis, we introduce MMSVG-2M, a multimodal dataset with two million richly annotated SVG assets, along with a standardized evaluation protocol for conditional SVG generation tasks. Extensive experiments show that OmniSVG outperforms existing methods and demonstrates its potential for integration into professional SVG design workflows.


<div align="center">
  <img src="assets/commands.png" alt="cmd" height="256px" />
  <img src="assets/omnisvg-teaser.gif" alt="Demo GIF" height="256px" style="margin-right: 10px;" />
</div>


<!-- ##  🧩 Dataset - MMSVG-2M -->

## Citation

```bibtex
@article{yang2025omnisvg,
  title={OmniSVG: A Unified Scalable Vector Graphics Generation Model}, 
  author={Yiying Yang and Wei Cheng and Sijin Chen and Xianfang Zeng and Jiaxu Zhang and Liao Wang and Gang Yu and Xinjun Ma and Yu-Gang Jiang},
  journal={arXiv preprint arxiv:2504.06263},
  year={2025}
}
```

## Acknowledgments
We thank the following excellent open-source works:
