# Drift City — open-world drift prototype

A real, working starting point for the game you described: open world, drift
physics, multiple cars, police that chase and shoot at you, a gun for
yourself, and a few missions. It's built with **Three.js** (JavaScript 3D)
wrapped in **Capacitor**, so the exact same code is both a browser game and a
real Android app.

## 1. Test it right now, no build needed
Open `www/index.html` in Chrome on your phone. The whole game runs right
there — drift physics, touch controls, police, shooting, missions — before
you touch Android Studio at all.

## 2. Build the APK — via GitHub Actions
Push to `main` and the included `.github/workflows/build.yml` builds the APK
automatically. Open the Actions tab, open the run, download the
`drift-city-debug-apk` artifact at the bottom of the page — that's your
installable APK. Allow "install unknown apps" on your phone to install it.

## 3. Controls
Steer/gas/brake buttons (or WASD/arrows), handbrake (HB/Space) for drift,
shoot (●/F) — also raises your wanted level.

## 4. Being honest about scope
A full GTA-style game is a multi-month studio project. This is a real,
testable prototype covering drift physics, cars, police AI, guns, and
missions — not a mockup. For a deeper build later, Unity (C#) is the
standard mobile-game answer (WheelCollider physics, NavMesh AI, asset
store) — this prototype's logic ports over conceptually if you go that
route. Kenney.nl has free (CC0) 3D car/city models if you want better
visuals than colored boxes.

## 5. Next steps
Tune `CAR_TYPES` in index.html, swap in real 3D models via GLTFLoader, add
sound, add real collision response, pool police cars/projectiles, add a
minimap.
