# ClearBuds: Wireless Binaural Earbuds for Learning-based Speech Enhancement

## Abstract
We present ClearBuds, the first  end-to-end hardware and software system that utilizes a neural network to enhance speech streamed from two wireless earbuds. Real-time speech enhancement for wireless earbuds  requires high-quality sound separation and background  cancellation, operating in real-time and on a mobile phone.  ClearBuds bridges state-of-the-art deep learning for blind audio source separation and in-ear mobile systems by making two key technical  contributions: 1) a new wireless earbud design capable of operating as a synchronized, binaural microphone array, and 2) a lightweight dual-channel speech enhancement neural network that runs on a mobile device. Results show that our wireless earbuds  achieve a  synchronization error less than 64 us and
our network has a runtime of 21.4 ms on an accompanying mobile phone. In-the-wild evaluation with eight users in  previously unseen indoor and outdoor multipath scenarios demonstrates that our neural network generalizes to learn both spatial and acoustic cues to  perform noise suppression and background speech removal. In a  user-study with 37 participants  who spent over 15.4  hours rating  1041   audio samples collected in-the-wild, our system achieves improved mean opinion score and background   noise  suppression.

## Contents
This directory contains the FPC (flexible printed circuit) design for ClearBuds. The FPC was designed in KiCAD 5.7.

- KiCAD design files are in shio_fpc folder.
- Fabrication output (Gerbers) are in shio_fpc/shio_rev_a_fab_v4. The suggested stack up is in shio_fpc/shio_stackup.xlsx. Suggested BOM is in shio_fpc/shio_BOM_rev_a_fab2_3.csv.
- Schematic PDF can be found at shio_fpc/

Errata: The design contains some errors that can be addressed in future revisions. The errors do not affect function, but do affect robustness. 1. Add 0.1uF decoupling capacitor to PDM mic (ICS-41350) Vcc. 2. Extend battery holder terminal pads further under solder mask to prevent pad tearout. 3. Consider using FR4 stiffener or RFPC to better support battery holder terminal pads to prevent pad tearout.


## Hardware Setup
1. Download KiCad
-  Go to https://www.kicad.org/download/
-  Download the latest for your environment
2. Open shio_fpc/shio.pro

![IMG_9959](https://user-images.githubusercontent.com/5505118/166155906-9f28a4dc-42b7-4920-86ec-815f177feb5e.jpeg)

