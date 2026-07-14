# Neural Sound Synthesis · Part 12 — Real-Time, Control & Frontiers

The final part of the [Neural Sound Synthesis](https://github.com/BrendanJamesLynskey/Neural_Sound_Synthesis) series. Turns from building models to deploying them: real-time streaming synthesis (RAVE), controllability, distribution-level evaluation, safety and provenance, and on-device efficiency — then folds all twelve parts back onto the single domain × family map the series opened with.

### [Launch App](https://brendanjameslynskey.github.io/Neural_Sound_Synthesis_12_Realtime_Control_Frontiers/)

Part of the [DSP & Music](https://github.com/BrendanJamesLynskey/DSP_and_Music) collection.

---

## What's inside

| Section | Content |
|---------|---------|
| **Real-Time & Streaming** | RAVE — streaming VAE + adversarial fine-tuning, causal/cached convolutions, the latency budget, nn~ for Max/PureData — with a **live latent-knob synth** |
| **Controllability** | Interpretable (DDSP), latent/attribute, symbolic, and text control surfaces; disentanglement and the precision-vs-generality tension |
| **Evaluation** | The full Fréchet Audio Distance formula, CLAP score, MOS/MUSHRA, KAD, and metric gameability — with an **interactive FAD explainer** |
| **Safety & Provenance** | Voice-cloning consent, deepfakes, audio watermarking (AudioSeal), C2PA content credentials, dataset & copyright questions |
| **On-Device & Efficiency** | Consistency models, distillation, quantization — the efficiency triangle |
| **The Map, Closed** | The series' domain × family map filled in, part-by-part — with a **navigable roadmap of the field** |
| **Frontier** | An honest list of open problems, and links back to Part 1 to revisit the map |

## Live demos (all synthesised in-browser, no audio files)

1. **Streaming latent knob** — a low-dimensional latent (z₁ brightness, z₂ harmonicity, z₃ register) drives a continuously-running Web Audio harmonic bank in real time; move a slider and the live timbre changes instantly, RAVE-style.
2. **FAD explainer** — two Gaussian point clouds (real vs generated) in a 2-D embedding space; move and reshape the generated cloud and watch the Fréchet Audio Distance and its mean/covariance split update live, collapsing to ~0 as the clouds overlap.
3. **Capability roadmap** — an interactive map of the 12 parts on a 2016 → now → frontier timeline; filter by open problem (real-time, control, long-form, evaluation, watermarking, on-device) and click any node for a summary and a link to that part.

## Technology

Single-file HTML/CSS/JS · Web Audio API · HTML5 Canvas · KaTeX · Palatino + Lucida Console · No external dependencies · No build step
