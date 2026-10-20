# EKG & Conduction Simulator

A bedside teaching tool by Warodom Phaenthong, M.D. One self-contained HTML file that runs in the browser,
with no installation and no data sent anywhere.

It simulates 60 rhythms and conduction patterns as a live 12-, 15- or 17-lead ECG, with a rhythm strip,
a picture of the heart and its conduction system, the electrodes on the body, and interventions to try.

## How the tracing is made

Since version 2.0.9 the ventricles and atria are a three-dimensional mesh of about 1,100 patches in their
real shape and position in the chest. The wave enters where the conduction system delivers it and spreads
through the muscle; each patch runs its own action potential; the ECG is the voltage difference between
touching patches, read by each electrode from where it sits. The *Mesh* view in the heart panel shows it.

The simulator is scored against real ECGs from PTB-XL (Wagner et al. 2020) and PTB-XL+ (Strodthoff et al.
2023), both CC BY 4.0. On the half of PTB-XL the model was never fitted to, 94.8% of measurements fall inside
the range of the matching group of real ECGs. The app contains no PTB-XL data.

It is a teaching aid for healthcare professionals, not a diagnostic device and not a substitute for clinical judgement.

`index.html` opens `ekg-simulator.html`. The changelog is behind the *What's new* button.

## Licence

Copyright (c) 2026 Warodom Phaenthong, M.D. Licensed under
[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/): share and adapt for non-commercial use,
with credit, under the same licence. See `LICENSE` and `NOTICE`.
