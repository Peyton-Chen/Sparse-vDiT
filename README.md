
<!-- <div align= "center">
    <h1> Official repo for Sparse-vDiT</h1>

</div> -->

<h3 align="center"><strong>Sparse-vDiT: Unleashing the Power of Sparse Attention to Accelerate Video Diffusion Transformers</strong></h3>

<div align="center">
<a href='https://arxiv.org/abs/2506.03065'><img src='https://img.shields.io/badge/arXiv-2506.03065-b31b1b.svg'></a> &nbsp;&nbsp;&nbsp;&nbsp;
</div>

## 🥳 What's New 
- [2025/06/03] 👋 Upload paper and init project. [Read](https://arxiv.org/abs/2506.03065)

<table>
  <tr>
    <td align="center">
      <em>Pretrain Model</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/pretrain_0.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>MInference</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/minference_0.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>Sparse-VideoGen</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/svg_0.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>Sparse-vDiT (1.76×)</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/sparsevdit_0.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center">
      <em>Pretrain Model</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/pretrain_1.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>MInference</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/minference_1.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>Sparse-VideoGen</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/svg_1.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>Sparse-vDiT (1.76×)</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/sparsevdit_1.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center">
      <em>Pretrain Model</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/pretrain_2.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>MInference</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/minference_2.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>Sparse-VideoGen</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/svg_2.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
    <td align="center">
      <em>Sparse-vDiT (1.76×)</em><br>
      <div style="width:180px; height:200px; overflow:hidden; display:flex; align-items:center; justify-content:center;">
        <img src="assets/video/sparsevdit_2.gif" style="min-width:100%; min-height:100%; object-fit:cover;">
      </div>
    </td>
  </tr>
</table>


## :pencil: To Do List
- [ ] Code and Checkpoints Release 
- [x] Technical Report


## 🏃 introduction

Sparse-vDiT is a sparsity acceleration framework for video diffusion transformers (vDiT). Through detailed analysis of attention maps in Video Diffusion Transformer (vDiT), we identify three recurring sparsity patterns: diagonal, multi-diagonal, and vertical-stripe structures. And even 3-6% attention heads can be skipped. Crucially, these patterns exhibit strong layer-depth and head-position correlations but show limited dependence on the input content. Leveraging these findings, we propose Sparse-vDiT, a sparsity acceleration framework for vDiT comprising: 1) Pattern-optimized sparse kernels that replace dense attention with computationally efficient implementations for each identified sparsity pattern. 2) An offline sparse diffusion search algorithm that selects the optimal sparse computation strategy per layer and head via hardware-aware cost modeling.

<p align="center">
    <img src="assets/pipeline.png" alt="Pipeline" width="890px" />
</p>

Our work demonstrates that latent structural sparsity in vDiTs can be systematically exploited for long video synthesis. Integrated into state-of-the-art vDiT models (CogVideoX1.5, HunyuanVideo, and Wan2.1), Sparse-vDiT achieves 2.09×, 2.38×, and 1.67× theoretical FLOP reduction, and actual inference speedups of 1.76×, 1.85×, and 1.58×, respectively, while maintaining high visual fidelity, with PSNR values reaching 24.13, 27.09, and 22.59.

<p align="center">
    <img src="assets/result.png" alt="Result" width="890px" />
</p>


<!-- :hammer: Installation -->


<!-- 🎯 Quick Start -->


## :notebook: Citation

```bibtex
@article{chen2025sparsevdit,
      title={Sparse-vDiT: Unleashing the Power of Sparse Attention to Accelerate Video Diffusion Transformers}, 
      author={Pengtao Chen and Xianfang Zeng and Maosen Zhao and Peng Ye and Mingzhu Shen and Wei Cheng and Gang Yu and Tao Chen},
      journal={arXiv preprint arXiv:2506.03065}, 
      year={2025}
}
```

## :dizzy: Acknowledgments
We thank the following excellent open-source works: [Sparse-VideoGen](https://github.com/svg-project/Sparse-VideoGen), [MInference](https://github.com/microsoft/MInference), [PAB](https://github.com/NUS-HPC-AI-Lab/VideoSys), [CogVideoX](https://github.com/THUDM/CogVideo), [HunyuanVideo](https://github.com/Tencent-Hunyuan/HunyuanVideo), [Wan2.1](https://github.com/Wan-Video/Wan2.1).

## :email: Contact
If you have any questions, please email [`Pengt.Chen@gmail.com`](mailto:Pengt.Chen@gmail.com).
