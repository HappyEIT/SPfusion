# SPfusion

In this project, we provide the more comprehensive Supplementary Materials for detailed illustrating (1) the sensitivity priors under the homogeneous distributions and inhomogeneous inclusions, (2) the settings of simulation training datasets, (3) the more visualization results and quantitative metrics of In-Distribution and Out-of-Distribution test datasets. This document is uploaded as a PDF file named 'TII_Supp Materials_SPfussion.pdf'. You can download it. 

# Brief introduction of SPfusion

The supervised deep learning methods for electrical impedance tomography (EIT) remains limited by hand-crafted and domain-specific instructions during training. The existing unsupervised solvers for EIT trade attention to the image domain with ignorance to physical natures in the electrical field. In this paper, we propose an unsupervised conditional diffusion model, referred to as SPfusion, for inhomogeneous sensitivity prior generation, which is utilized as the system matrix to solve EIT inverse problem. The conditional diffusion model first undergoes coarse training to ensure stable generation, followed by a dedicated fine training to sharpen detailed fidelity. In SPfusion, We propose a novel dual-domain denoising network, named DDSP-Net, that introduces the dual-domain Cartesian-based and polar-based coordinates dual-domain Transformer to efficiently capture multi-scale latent representations. Additionally, the measurement conditional attention-based Decoder is proposed to fully preserve dual-domain long-range dependencies. SPfusion achieves accurate noise estimation, high-fidelity detail generation of the inhomogeneous sensitivity prior, as well as high-quality image reconstructions based on model-driven methods. Experiments conducted on simulation data, real-world measurements, and publicly available benchmark demonstrate that SPfusion outperforms supervised/unsupervised and previous diffusion-based methods in terms of reconstruction accuracy and stability.

# Main contributions

(1) We propose a novel diffusion-based inhomogeneous sensitivity prior generation method based on the homogeneous sensitivity as boundary condition and the measured voltage as guided condition, named \textbf{SPfusion}.

(2) We propose a novel \textbf{DDSP-Net} with three novel Transformer-based modules, which are PixelFormer based on Cartesian coordinate, PolarFormer based on polar coordinates, and $U$-conditional cross-attention. 

(3) The visual reconstructions and quantitative metrics, both on in-distribution and out-of-distribution data, show that our SPfusion can effectively improve the quality of reconstruction compared with state-of-the-art methods.
