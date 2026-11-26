# Radiant Christmas Tree · Merry Christmas

A browser-based 3D interactive Christmas tree page with gesture control, photo slideshow, music, and snowfall.

## Try it online

- Desktop (full experience): https://cchantelhu.github.io/christmas-tree/
- Mobile lite: https://cchantelhu.github.io/christmas-tree/?lite=1

On phones, Safari or Chrome is recommended. 

## How to use

1. Open the page and click once to enter.
2. Add photos in the gallery panel.
3. Click the camera / gesture button at the top right and allow camera access.
4. Use these gestures in front of the camera:
   - Open palm: Christmas tree particles bloom.
   - Closed fist: particles return to the tree shape and stay clustered.
   - Pinch thumb and index finger, then release: switch to the next photo; after the last photo, it loops to the first.
5. Drag with the mouse or use touch to adjust the view.

## Privacy

- Uploaded photos are stored in this site’s local database on the current device and browser; they are not written into this GitHub repository.
- This version has no feature that uploads photos to a server or sends them to the site owner; photos are shown via local browser object URLs.
- The camera feed is processed by MediaPipe hand tracking in the browser; the current code does not send the camera feed to a server.
- Photos persist when you reopen the page on the same device and browser profile; anyone sharing that browser profile may see them.
- Clearing this site’s data in the browser deletes locally saved photos. Photos do not sync automatically across devices or browser profiles.

## Repository contents

This repository contains static build files ready for GitHub Pages:

- `index.html`: page entry.
- `assets/`: built JavaScript and CSS.
- `mediapipe/`: gesture recognition runtime files.
- `audio/`: page music assets.

This repository does not include the original React/TypeScript source; interaction logic lives in the built JavaScript.

## Publishing

GitHub Pages publishes from the root of the `main` branch. After changes are pushed, GitHub Actions builds and deploys automatically.

## Source

This repository is forked from [nobody-r/christmas-tree](https://github.com/nobody-r/christmas-tree), with additions for gesture-driven photo slideshow, interaction hints, countdown boundary fixes, and a mobile lite link. See the upstream repository for the original project notes and license.
