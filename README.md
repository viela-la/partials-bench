# Partials Bench

An additive-synthesis playground that runs in the browser. Build sounds out of sine waves (partials), see the waveform and spectrum, shape them with a drawable filter, synthesize vowels, and analyze your own voice with the microphone.

**Live app:** https://YOUR-USERNAME.github.io/partials-bench/

## Features

- **Partials** — type any frequency and amplitude, paste many at once, mute or delete each one.
- **Generators** — harmonic series (f, 2f, 3f… with sawtooth, square or triangle-like amplitudes) and random frequencies in a range.
- **Waveform** — zoom from 1 ms to 20 s, drag to pan, scroll or pinch to zoom.
- **Spectrum** — linear or log frequency axis.
- **Filter** — low-pass, high-pass, band-pass, notch, peak, or a custom curve you draw by dragging on the spectrum. Optional automatic sweep.
- **Vowel synth** — 10 English vowels for man, woman and child voices (Peterson & Barney, 1952 formant averages). Click a vowel, drag on the vowel chart, or type a sequence such as `ee eh ah aw oo` and press Speak.
- **Microphone** — live pitch, spectrum and vowel detection; capture a sound as partials; let the synth follow your pitch and vowel; or capture your voice so every vowel is rebuilt from your pitch, voice color and formant scale.

## Running it

It is a single HTML file with no build step and no dependencies.

- Open `index.html` in Chrome, or
- Visit the GitHub Pages link above.

The microphone needs a secure page (`https://` or a local file) and your permission. Wear headphones when the synth follows your voice to avoid feedback.

## How it works

Each partial is a Web Audio sine oscillator with its own gain. The filter and vowel synth set those gains from a frequency response, so the waveform and spectrum plots show exactly what you hear (amplitudes only; filter phase is not modeled). Pitch detection uses the YIN algorithm; formants are estimated by fitting the vowel model to the measured harmonic levels.
