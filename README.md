# Free Space Path Loss & Link Budget Calculator

A free, browser-based RF tool for computing **free space path loss (FSPL)** and running a quick **RF link budget**. No install, no sign-up, no data leaves your browser — results update live as you type.

**Online tool:** https://xiaokeni2.github.io/free-space-path-loss-calculator/

## What it does

- **FSPL calculator** — enter frequency (Hz / kHz / MHz / GHz) and distance (m / km / mile) to get path loss in dB.
- **Link budget calculator** — enter TX power, antenna gains and extra losses to get received power P<sub>r</sub> and link margin against a configurable RX sensitivity (default −100 dBm).
- One-click presets: 2.4 GHz Wi-Fi, 5.8 GHz Wi-Fi, 12 GHz satellite downlink.
- Single-file, dependency-free frontend with a dark engineering UI; works on mobile.

## Formulas

FSPL (dB) = 20·log₁₀(d) + 20·log₁₀(f) + 32.44

where d is distance in **km** and f is frequency in **MHz**.

Received power: P<sub>r</sub> (dBm) = P<sub>tx</sub> + G<sub>tx</sub> + G<sub>rx</sub> − FSPL − L

Link margin: P<sub>r</sub> − RX sensitivity (positive margin means the link closes).

## Usage

Open https://xiaokeni2.github.io/free-space-path-loss-calculator/ in any modern browser. Pick a frequency preset or type your own values — the FSPL result and the link budget (received power, margin) update instantly.

## Related

More RF tools: [BRIDZA RF Component Selector](https://rf.bridza.com/) · [OCXO / TCXO Parametric Search](https://xiaokeni2.github.io/rf-component-selector/)
