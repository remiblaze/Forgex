# Forgex: channel utility & stereo toolkit

![Forgex free channel utility & stereo toolkit UI](https://raw.githubusercontent.com/RemiBlaze/Forgex/main/forgex-ui-screenshot.png)

**The Swiss army knife that goes on every track.**

Gain, pan, stereo width, phase, channel routing, low-end mono, and safety limiting in one dead-simple utility, with real-time correlation and level metering so you always know what your signal is doing.

**macOS** (Apple Silicon and Intel): AU, VST3, CLAP, AAX, Standalone. Signed and notarized by Apple.

**Windows** 10 and 11, 64-bit: VST3, CLAP, Standalone. Authenticode signed.

AAX ships on macOS only.

---

## 🚀 Download & Install

Go to the [latest release](https://github.com/RemiBlaze/Forgex/releases/latest) and pick your platform.

**macOS**
1. Download **`Forgex_Installer.pkg`**.
2. Double-click it and follow the installer. It is signed and notarized by Apple, so it installs cleanly with no security warnings.
3. Restart your DAW and rescan plug-ins. Forgex appears under **Remi Blaze**.

**Windows 10 and 11, 64-bit**
1. Download **`Forgex_Installer.exe`**.
2. Run it and follow the installer. It is Authenticode signed.
3. Restart your DAW and rescan plug-ins. Forgex appears under **Remi Blaze**.

No dongle and no extra account on either platform.

Full guide: **[remiblaze.com/support](https://remiblaze.com/support/)**.

---

## 🎛️ Features
- **Gain**: smoothed level control from -100 dB to +24 dB
- **Pan**: full left/right pan with **Balance** or **Constant Power** pan law
- **Stereo Width**: 0% (mono) to 200% (extra wide)
- **Phase Invert**: independent left and right channel polarity flip
- **Mono**: sum to mono for instant mono compatibility checks
- **Channel Routing**: Stereo, Swap L/R, Left Only, Right Only, Mid Only, Side Only
- **DC Filter**: removable 5 Hz high-pass to strip DC offset
- **Low-End Monomizer**: sums frequencies below an adjustable crossover (20–500 Hz) to mono
- **ISP Limiter**: inter-sample peak limiting with a -0.1 dB ceiling
- **Bypass**: clean A/B against the source
- **Correlation Meter**: real-time stereo phase readout with warning indicator
- **Input / Output Meters**: stereo level metering with ballistic smoothing
- **A/B Comparison**: store and recall two complete states
- **Randomize**: shake up gain, pan, and width
- **User Presets**: save and load your own settings to disk

---

## 🔬 Under the Hood
- **Low-End Monomizer** uses a 4th-order Linkwitz-Riley crossover to split the signal, mono the lows, and phase-coherently recombine.
- **DC filter** is a 5 Hz high-pass that removes DC offset introduced by nonlinear stages upstream.
- **ISP Limiter** performs inter-sample peak detection with instant attack and ~50 ms release, holding a -0.1 dB ceiling; when disabled, a transparent soft clipper guards the output.
- **Width** is implemented in the mid/side domain for mono-compatible stereo control.

---

## 💻 System Requirements

**macOS**
- macOS 15.0 or later
- Apple Silicon or Intel Mac (Universal Binary)
- An AU, VST3, CLAP or AAX host

**Windows**
- Windows 10 or Windows 11, 64-bit
- A VST3 or CLAP host

---

## 🎚️ Factory Presets (15)

| Preset | Best For |
|--------|----------|
| Init | Clean starting point |
| Mono Check | Instant mono compatibility check |
| Wide | Gentle stereo widening |
| Extra Wide | Maximum width |
| Narrow | Tighten the stereo image |
| Left Only | Solo the left channel |
| Right Only | Solo the right channel |
| Mid Solo | Solo the mid (center) |
| Side Solo | Solo the sides |
| Phase Flip | Flip both channel polarities |
| Pocket Anchor | Focused low-end with slight narrowing |
| Sassy Lead Width | Wide, trimmed lead |
| High-Hat Shimmer | Widened hats with a polarity twist |
| Gain Stage -6 | Quick -6 dB gain stage |
| Remi Blaze Utility | Signature everyday utility setting |

---

## 🐛 Bugs & Issues
Open an issue on the **[Issues](https://github.com/RemiBlaze/Forgex/issues)** tab with your macOS or Windows version, DAW + version, and steps to reproduce.

---

## 📄 License & Credits
- **Plugin page:** [remiblaze.com/plugins/forgex/](https://remiblaze.com/plugins/forgex/).
- **Developer:** [Remi Blaze](https://remiblaze.com).
- **Framework:** [JUCE](https://juce.com).
- **License:** free under a proprietary [Freeware License](LICENSE) (see also our [terms](https://remiblaze.com/terms/)). Reverse-engineering, repackaging, binary redistribution, or reselling the compiled installer is strictly prohibited.

---

## Trademarks

All product names, company names, and logos mentioned herein are trademarks or registered trademarks of their respective owners. Any such references are used for descriptive or compatibility purposes only and do not imply affiliation with, endorsement by, or sponsorship from their owners.

VST is a trademark of Steinberg Media Technologies GmbH, registered in Europe and other countries.

Apple, macOS, Audio Units (AU), and Apple Silicon are trademarks of Apple Inc., registered in the U.S. and other countries.

AAX, Avid, and Pro Tools are trademarks or registered trademarks of Avid Technology, Inc. in the U.S. and other countries.

Microsoft and Windows are trademarks of the Microsoft group of companies.
