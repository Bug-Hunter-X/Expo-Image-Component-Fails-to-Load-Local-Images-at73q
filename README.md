# Expo Image Component Local Image Loading Issue

This repository demonstrates a bug where the Expo `Image` component fails to load local images even when the URI is correct and the image file exists within the project's assets.

The issue is characterized by a lack of informative error messages, making debugging challenging.  Potential causes include asset path resolution problems or caching conflicts.

The `bug.js` file shows the problematic code, while `bugSolution.js` presents a potential solution, although a definitive fix might require further investigation into Expo's asset handling mechanism.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Start the Expo development server.
4. Observe the image component's failure to load the local image.

## Solution

The proposed solution (in `bugSolution.js`) involves ensuring the image path is correctly relative to the main application directory. Additionally, it demonstrates various methods to load images using the `Image` component, helping to isolate and understand potential causes for the loading failure.