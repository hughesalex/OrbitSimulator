# Orbit Simulator

An interactive sandbox for learning how orbits work, in the style of the [Orrery](https://hughesalex.github.io/orrery/orrery.html).

A spacecraft circles Earth. Click anywhere on its orbit to plan a burn there, then drag the coloured handles (or use the + and − buttons) to push prograde, normal or radial, as with maneuver nodes in Kerbal Space Program. The dashed blue path shows where the craft will go after the burn, and the Orbit panel compares apoapsis, periapsis, eccentricity, inclination and the other orbital elements before and after. Tap any row in that panel for an explanation.

Starting orbits include a low equatorial orbit, the space station's orbit, a geostationary transfer orbit, geostationary, Molniya, sun-synchronous, a suborbital hop and an escape trajectory.

The physics is exact two-body motion (Kepler's laws) with instant burns. There is no air drag, no Moon and no effect of Earth's equatorial bulge yet.

## Files

`orbit-simulator.html` is the whole app: a single file that works offline. Open it straight from disk in a browser.

It is built from `src/orbit-simulator.html` by `build.sh`, which embeds the files in `vendor/` (fonts, three.js r128 and its OrbitControls, and the Earth map from Solar System Scope, CC BY 4.0, all taken from the Orrery). Edit the source, then run `bash build.sh`.
