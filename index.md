---
layout: home
title: Home
---

<div class="hero">
  <h1>{{ site.title }}</h1>
  <p class="tagline">{{ site.description }}</p>

  <p class="links">
    <a href="{{ site.github }}">GitHub</a>
    <a href="{{ site.linkedin }}">LinkedIn</a>
    <a href="{{ site.cgpage }}">VC Bonn</a>
    <a href="{{ site.email }}">Email</a>
  </p>
</div>

## Selected projects

<div class="cards">

  <div class="card">
    <h3>Project 1: Transformer-Based Real-Time Inpainting [WACV 2026]</h3>
    <div class="meta">Patch-based transformer • real-time inpainting • spatiotemporal embeddings</div>
    <p>
      High-quality 3D streaming from multiple cameras is crucial for immersive experiences in many AR/VR applications. The limited number of views – often due to real-time constraints – leads to missing information and incomplete surfaces in the rendered images. Existing approaches typically rely on simple heuristics for the hole filling, which can result in inconsistencies or visual artifacts. We propose to complete the missing textures using a novel, application-targeted inpainting method independent of the underlying representation as an image-based post-processing step after the novel view rendering. The method is designed as a standalone module compatible with any calibrated multi-camera system. For this we introduce a multi-view aware, transformer-based network architecture using spatio-temporal embeddings to ensure consistency across frames while preserving fine details. Additionally, our resolution-independent design allows adaptation to different camera setups, while an adaptive patch selection strategy balances inference speed and quality, allowing real-time performance. We evaluate our approach against state-of-the-art inpainting techniques under the same real-time constraints and demonstrate that our model achieves the best trade-off between quality and speed, outperforming competitors in both image and video-based metrics.
    </p>
    <p class="badges">
      <span>Inpainting</span><span>3D reconstruction</span><span>Real-time</span>
    </p>
    <p>
      <a href="https://github.com/vc-bonn/transformer-based-inpainting">Code</a> ·
      <a href="">Paper (coming soon)</a> ·
      <a href="">Video (coming soon)</a>
    </p>
  </div>

  <div class="card">
    <h3>Project 2 — NeRFs are Mirror Detectors [WACV 2025 Oral]</h3>
    <div class="meta">Neural rendering • reflections • failure detection</div>
    <p>
      While neural radiance fields (NeRF) led to a breakthrough in photorealistic novel view synthesis, handling mirroring surfaces still denotes a particular challenge as they introduce severe inconsistencies in the scene representation. Previous attempts either focus on reconstructing single reflective objects or rely on strong supervision guidance in terms of additional user-provided annotations of visible image regions of the mirrors, thereby limiting the practical usability. In contrast, in this paper, we present NeRF-MD, a method which shows that NeRFs can be considered as mirror detectors and which is capable of reconstructing neural radiance fields of scenes containing mirroring surfaces without the need for prior annotations. To this end, we first compute an initial estimate of the scene geometry by training a standard NeRF using a depth reprojection loss. Our key insight lies in the fact that parts of the scene corresponding to a mirroring surface will still exhibit a significant photometric inconsistency, whereas the remaining parts are already reconstructed in a plausible manner. This allows us to detect mirror surfaces by fitting geometric primitives to such inconsistent regions in this initial stage of the training. Using this information, we then jointly optimize the radiance field and mirror geometry in a second training stage to refine their quality. We demonstrate the capability of our method to allow the faithful detection of mirrors in the scene as well as the reconstruction of a single consistent scene representation, and demonstrate its potential in comparison to baseline and mirror-aware approaches.
    </p>
    <p class="badges">
      <span>NeRF</span><span>Reflections</span><span>Analysis</span>
    </p>
    <p>
      <a href="https://github.com/vc-bonn/nerfs-are-mirror-detectors">Code</a> ·
      <a href="https://arxiv.org/abs/2501.04074">Paper</a>
    </p>
  </div>

  <div class="card">
    <h3>Project 3 — TraM-NeRF [CGF 2024]</h3>
    <div class="meta">Neural rendering • reflections • ray tracing</div>
    <p>
      Implicit representations like neural radiance fields (NeRF) showed impressive results for photorealistic rendering of complex scenes with fine details. However, ideal or near-perfectly specular reflecting objects such as mirrors, which are often encountered in various indoor scenes, impose ambiguities and inconsistencies in the representation of the re-constructed scene leading to severe artifacts in the synthesized renderings. In this paper, we present a novel reflection tracing method tailored for the involved volume rendering within NeRF that takes these mirror-like objects into account while avoiding the cost of straightforward but expensive extensions through standard path tracing. By explicitly modelling the reflection behaviour using physically plausible materials and estimating the reflected radiance with Monte-Carlo methods within the volume rendering formulation, we derive efficient strategies for importance sampling and the transmittance computation along rays from only few samples. We show that our novel method enables the training of consistent representations of such challenging scenes and achieves superior results in comparison to previous state-of-the-art approaches.
    </p>
    <p class="badges">
      <span>NeRF</span><span>Reflections</span><span>Ray Tracing</span>
    </p>
    <p>
      <a href="https://github.com/Rubikalubi/TraM-NeRF">Project page</a> ·
      <a href="https://onlinelibrary.wiley.com/doi/10.1111/cgf.15163">Paper</a>
    </p>
  </div>

</div>

## About

More coming soon...
