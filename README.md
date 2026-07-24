# Foresight

An AI narrator for the world in front of you, built first for blind and low-vision users, starting with the Nigerian street environment (okadas, potholes, gutters, POS stands, road bumps) that most vision models aren't trained to prioritize.

Foresight watches through a phone camera and speaks only when something matters, be it a hazard, a person, a meaningful change instead of narrating everything constantly. The hard problem isn't detecting objects. It's deciding **what's worth saying, and when.**

## Status: early prototype

This is a day-one working prototype, not a finished product. Right now:

- Runs entirely in a phone browser, no app install needed
- Takes a camera frame every few seconds
- Sends it to a vision-language model with strict instructions: describe only what matters, skip everything else
- Speaks the result out loud through the phone

What's not built yet:
- No tuning for Nigerian-specific hazards (okada, danfo, open gutters, road bumps) — not yet tested against real local street scenes
- No spatial audio / distance cues
- No offline or low-connectivity handling
- No real user testing yet with blind or low-vision users

## Why this exists

Existing tools like Seeing AI and Be My Eyes are good but slow and verbose, they describe everything instead of prioritizing what matters in the moment, and they're built and tested mostly in Western environments. Foresight starts from the opposite direction: fewer words, better judgment about timing, and built with the Nigerian street environment as a first-class use case rather than an afterthought.

## Try it

Open `index.html` in a phone browser (Chrome/Safari), grant camera access, and tap the button to start narration. Requires an internet connection.

## Roadmap

1. Validate the vision model against real Nigerian street scenes (potholes, okadas, gutters, POS kiosks)
2. Tune narration frequency and "what's worth saying" logic based on real testing
3. Get feedback from actual blind/low-vision users
4. Explore dedicated hardware (camera + bone-conduction earpiece) once the software is proven.

## License

TBD
