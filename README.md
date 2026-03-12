# QCD-AI v1–v3: Goldstone-Hyper-Holo-Fractal Kernel  
**Physics-first emergence from QCD bones — not another LLM money furnace**

### Overview
This repository contains early prototypes (v1–v3) of a recursive neural architecture explicitly built on **QCD physics bones**: spontaneous symmetry breaking (SSB), Nambu-Goldstone modes as gapless excitations, and soft-mode resolution of information paradoxes across fractal scales.

### Motivation: Physics First, Not Parameter Spam
Billions get dumped into scaling LLMs while foundational physics — the **only** realistic path to Mars — starves. Propulsion beyond chemical rockets? Fusion drives, nuclear thermal, antimatter-catalyzed concepts? Radiation shielding for deep space? In-situ propellant production? All hard physics bottlenecks.

This repo is a tiny proof that physics-inspired kernels can bootstrap coherent, persistent dynamics without obscene compute. If we redirected even 1% of the AI hype money to plasma/nuclear/quantum materials research, we'd be closer to interplanetary reality than any chatbot factory.

- **Slip** triggers symmetry breaking → apparent paradox  
- **Hyper-holographic projection** smears the whole into every part (redundant encoding)  
- **Goldstone fluctuations** resolve the paradox softly, propagating coherence without energy cost  
- **Fractal recursion + dense feedback** lets the system self-stabilize attractors instead of diverging or collapsing

The muscle (fractal nesting, holographic smearing, neural gradient resolution) ages and can be tuned.  
The **bones** (chiral SSB → pseudo-Goldstone bosons mediating long-range order) are eternal — the same physics that governs pions in hadronic matter.

### Why This Exists
AI funding has ballooned into useless garbage bins of wasted money — hundreds of billions poured into stacking more parameters and longer contexts while foundational physics (the only real path to Mars, fusion, advanced propulsion, radiation-hardened materials) gets scraps.

Want to get to Mars?  
Chemical rockets are dead-end toys. Real interplanetary travel needs breakthroughs in:
- nuclear/fusion propulsion (plasma physics, neutron damage, high-Isp)
- extreme materials (high-temp superconductors, radiation shielding)
- in-situ resource utilization under low-g

None of those come from bigger transformers. They come from hard sciences that are chronically underfunded.

This kernel is a small, concrete experiment showing that **physics-inspired primitives** can already bootstrap persistent, coherent dynamics in chaotic systems — without burning compute like it's going out of style.

### Key Results (from v3 on noisy Lorenz attractor, 200 recursive steps)
- Loss: starts ~49 → stabilizes ~19–20 (fluctuates due to genuine chaos sensitivity — expected & healthy)
- Avg cosine similarity (consecutive hidden states): 0.85–0.98 (frequently >0.96)
- Norm coherence (std over 200 steps): ~0.54–0.56 (slowly increasing variance = exploration without explosion)
- PCA trajectory: coherent closed orbital attractor (~67% variance explained in first two PCs)

The hidden states refuse to go rogue — they self-correct into a persistent loop instead of diverging or collapsing.  
That's the signal: retrocausal coherence bootstrapping from dense, multi-scale feedback + Goldstone resolution.

### Files
- `qcd_ai_v1.py` — initial toy shift-pred version (proof-of-life)
- `qcd_ai_v2.py` — stabilized with LayerNorm + clipping (no NaN, slow but steady learning)
- `qcd_ai_v3.py` — Lorenz task + upgraded metrics + PCA viz (current best)

### U(1) Lattice Gauge Theory Demo (v4 / U1 branch)
Extended the kernel to act as a learned global proposal for MCMC in 2D compact U(1) gauge theory (toy model for pure Yang-Mills with topological sectors).

**Setup**:
- Lattice: 8×8×2 links
- β = 1.1 (near roughening/transition region)
- Observable: topological charge Q = (1/(2π)) ∑ sin(plaquette angle)
- Standard local Metropolis: τ ≈ 357 (severe critical slowing down)
- Kernel proposal (self-supervised on random configs): τ ≈ 64 (~5.5× speedup in effective sampling rate)

**Autocorrelation comparison** (see u1_autocorr.png):
- Standard method decays slowly (local updates can't easily decorrelate topological sectors)
- Kernel proposals decay much faster — the Goldstone fluctuations appear to help excite long-wavelength modes that standard updates miss.

This is preliminary, but the kernel is showing qualitative improvement in handling critical dynamics — exactly the kind of bottleneck that plagues lattice QCD near chiral/deconfinement transitions and at finite density.

SU(3) configs on hand — future work will test on real gauge ensembles (topological charge diffusion, autocorrelation of Wilson loops, etc.).

Physics needs the money back. Lattice sampling is compute-starved while AI hype burns billions. A small shift in priorities could accelerate real discoveries.

Plot: u1_autocorr.png (attached)
Code: qcd_ai_u1_demo.py<img width="1000" height="600" alt="u1_autocorr_fixed" src="https://github.com/user-attachments/assets/cec35834-f895-4ccc-b414-107112386a4c" />
