# ComfyUI Dataset Generation Pipeline

[中文版](./README_CN.md) | English

## Overview

This project showcases synthetic data generation results: deploying ComfyUI on a local server to generate synthetic datasets for intelligent security systems. Includes image-to-image and image-to-video workflows.

## Project Content

<table align="center">
  <tr>
    <th>Type</th>
    <th>Model</th>
    <th>Quantity</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td>Image-to-Image</td>
    <td>FLUX.2</td>
    <td>40,000</td>
    <td>Object detection (people, vehicles, pets)</td>
  </tr>
  <tr>
    <td>Image-to-Video</td>
    <td>Wan2.2</td>
    <td>10,000</td>
    <td>Abnormal behavior detection (climbing)</td>
  </tr>
</table>

## Build Workflows in ComfyUI

### Image-to-Image Workflow
<p align="center">
  <img src="./img/workflow/FLUX2.png" alt="Image-to-Image Workflow" width="800"/>
</p>

**Model**: FLUX.2
**Prompt**: Replace the existing cats or dogs in the image with a significantly reduced-scale cat or dog, placed on the floor or furniture, clarity consistent with the original image, realistic pose, natural integration, correct perspective, lighting, and shadows.
**Output**: 40,000 surveillance-style cat/dog images

### Image-to-Video Workflow
<p align="center">
  <img src="./img/workflow/Wan2_2.png" alt="Image-to-Video Workflow" width="800"/>
</p>

**Model**: Wan2.2
**Prompt**: surveillance camera view, static CCTV angle, adult male or adult female climbing from inside the room out through a window or climbing over a balcony railing to the outside, non-violent, non-sexual, cautious or accidental motion, residential apartment or house balcony/window setting, realistic lighting, realistic human anatomy and movement, uncluttered background, realistic physical interaction, obeys collision with environment, natural motion
**Output**: 10,000 videos of climbing behavior

## Generated Examples

### Image Samples
<p align="center">
  <img src="./img/samples/cat2.png" alt="Generated Image Sample 1" width="400" style="margin: 10px;"/>
  <img src="./img/samples/dog2.png" alt="Generated Image Sample 2" width="400" style="margin: 10px;"/>
</p>

### Video Samples
<p align="center">
  <em>Click on thumbnails below to play videos</em>
</p>
<p align="center">
  <!-- First video: thumbnail links to video file -->
  <a href="./video/climbing1.mp4" title="Click to play climbing1.mp4">
    <img src="./img/thumbnail/climbing1_thumb.png" alt="climbing1" width="400" />
  </a>
  &nbsp;&nbsp;&nbsp;
  <!-- Second video: thumbnail links to video file -->
  <a href="./video/climbing2.mp4" title="Click to play climbing2.mp4">
    <img src="./img/thumbnail/climbing2_thumb.png" alt="climbing2" width="400" />
  </a>
</p>
