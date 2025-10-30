---
title: AI Video Generation
categories:
- General
---

Recent breakthroughs like Sora by OpenAI and Veo 3 by Google DeepMind have flooded social feeds with jaw-dropping AI-generated videos — setting the bar higher than ever for text-to-video generation. Meanwhile, the open-source community is rapidly catching up, releasing powerful models that anyone can run on a decent GPU. But flashy demos don't reveal the hidden costs: how much energy and compute time does it really take to make just a few seconds of footage?

![video](https://cdn-uploads.huggingface.co/production/uploads/67ecf57f1f0e7c18eec758c9/9WAlfMMlteiFlmEj_EYf2.mp4)

The authors of this paper ran energy benchmarking for some of the latest open-source text-to-video models — including Mochi-1-preview, CogVideoX-5b, WAN2.1-T2V-1.3B-Diffusers, AnimateDiff, and others — and measured how much energy it takes to produce a short video.

They found huge differences in energy use between models — sometimes by orders of magnitude. For example, AnimateDiff uses barely 0.11 Wh on GPU to produce a short clip, while WAN2.1-T2V-14B burns almost 94 Wh just on the GPU for a single video.

![visualization](https://cdn-uploads.huggingface.co/production/uploads/67ecf57f1f0e7c18eec758c9/5PPYryLkPsoaI8HI2B6qW.mp4)

This range represents the difference between 50 minutes of a 10W LED bulb and  7–10 full smartphone charges!

Check out the [blog post](https://huggingface.co/blog/jdelavande/text-to-video-energy-cost) and [full paper](https://arxiv.org/pdf/2509.19222) for more details.

By: Julien Delavande, Regis Pierrard, Sasha Luccioni
