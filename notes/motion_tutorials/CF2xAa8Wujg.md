# CF2xAa8Wujg
(source: transcript)

**Recipe for the After Effects Tutorial**

**Text Animation**

1. Create a new composition with the following settings:
	* Resolution: 1080p
	* Frame Rate: 60fps
	* Duration: 60 seconds
2. Create a new text layer with the following settings:
	* Font: Open Sans
	* Font Size: 48pt
	* Color: #333333
	* Text: "Motion design is not difficult, but people on the internet have just made it unnecessarily complex."
3. Add a new animation to the text layer with the following settings:
	* Type: Scale
	* Easing: Ease In (30%, 90%)
	* Keyframe 1: 0s, 100% scale
	* Keyframe 2: 10s, 150% scale
	* Keyframe 3: 20s, 100% scale
4. Add a new animation to the text layer with the following settings:
	* Type: Position
	* Easing: Ease Out (30%, 90%)
	* Keyframe 1: 0s, 0% position
	* Keyframe 2: 10s, 50% position
	* Keyframe 3: 20s, 0% position

**Motion Blur**

1. Add a new effect to the text layer with the following settings:
	* Effect: Motion Blur
	* Blur Type: Directional
	* Blur Amount: 50%
	* Blur Radius: 10px

**Glow**

1. Add a new effect to the text layer with the following settings:
	* Effect: Drop Shadow
	* Shadow Color: #FFFFFF
	* Shadow Opacity: 50%
	* Shadow Distance: 10px
	* Shadow Size: 10px

**Background Animation**

1. Create a new solid layer with the following settings:
	* Color: #333333
	* Opacity: 50%
2. Add a new animation to the solid layer with the following settings:
	* Type: Scale
	* Easing: Ease In (30%, 90%)
	* Keyframe 1: 0s, 100% scale
	* Keyframe 2: 10s, 150% scale
	* Keyframe 3: 20s, 100% scale

**Camera Null Move**

1. Create a new null object with the following settings:
	* Position: 0, 0, 0
	* Scale: 100%
2. Add a new animation to the null object with the following settings:
	* Type: Position
	* Easing: Ease Out (30%, 90%)
	* Keyframe 1: 0s, 0% position
	* Keyframe 2: 10s, 50% position
	* Keyframe 3: 20s, 0% position

**UI Mockup Handling**

1. Create a new composition with the following settings:
	* Resolution: 1080p
	* Frame Rate: 60fps
	* Duration: 60 seconds
2. Import a UI mockup image with the following settings:
	* Image: UI mockup image
	* Scale: 100%
3. Add a new animation to the UI mockup image with the following settings:
	* Type: Scale
	* Easing: Ease In (30%, 90%)
	* Keyframe 1: 0s, 100% scale
	* Keyframe 2: 10s, 150% scale
	* Keyframe 3: 20s, 100% scale

**Typography Sizes/Fonts**

1. Use the following font sizes and fonts:
	* Open Sans: 48pt
	* Arial: 24pt

**Sound**

1. Import a sound file with the following settings:
	* Sound: Sound file
	* Volume: 50%

**Reproducing in Remotion**

To reproduce this tutorial in Remotion, you can use the following code:
```jsx
import { interpolate, spring } from 'remotion';

const text = 'Motion design is not difficult, but people on the internet have just made it unnecessarily complex.';
const font = 'Open Sans';
const fontSize = 48;
const color = '#333333';

const textLayer = {
  x: 0,
  y: 0,
  scale: 1,
  rotation: 0,
  opacity: 1,
};

const backgroundLayer = {
  x: 0,
  y: 0,
  scale: 1,
  rotation: 0,
  opacity: 0.5,
};

const uiMockupLayer = {
  x: 0,
  y: 0,
  scale: 1,
  rotation: 0,
  opacity: 1,
};

const animation = () => {
  const time = interpolate(0, 60, 0, 1);

  const textAnimation = spring({
    x: 0,
    y: 0,
    scale: 1,
    rotation: 0,
    opacity: 1,
  });

  const backgroundAnimation = spring({
    x: 0,

**Recipe for the After Effects SaaS Tutorial**

**1. Background Animation**

- Set the background layer to a solid color (RGB: 0, 0, 0)
- Add a gradient layer with the following settings:
  - Gradient type: Linear
  - Gradient direction: 90°
  - Gradient stops:
    - Stop 1: RGB: 0, 0, 0 (0%)
    - Stop 2: RGB: 255, 255, 255 (100%)
  - Mask: Ellipse with a 50% opacity
- Set the animation to a simple fade-in effect:
  - Keyframe 1: 0s, 0% opacity
  - Keyframe 2: 10s, 100% opacity

**2. Typography**

- Create a new text layer with the following settings:
  - Font: Open Sans
  - Font size: 48pt
  - Text: "What do I want the viewer to feel in this moment?"
  - Text color: RGB: 255, 255, 255
- Add a text animator with the following settings:
  - Text animator type: Scale
  - Scale: 100% to 150% over 5s
  - Ease: Ease-in

**3. Motion Blur**

- Enable motion blur on the text layer:
  - Motion blur type: Basic
  - Motion blur amount: 50%
  - Motion blur duration: 5s

**4. Glow**

- Add a glow effect to the text layer:
  - Glow type: Basic
  - Glow color: RGB: 255, 255, 255
  - Glow size: 10px
  - Glow opacity: 50%

**5. Transitions**

- Add a transition effect to the text layer:
  - Transition type: Fade
  - Transition duration: 2s

**6. UI Mockup Handling**

- Create a new composition with the following settings:
  - Composition size: 1920x1080
  - Frame rate: 30fps
- Add a new solid layer with the following settings:
  - Layer size: 1920x1080
  - Layer color: RGB: 255, 255, 255
- Add a new text layer with the following settings:
  - Font: Open Sans
  - Font size: 24pt
  - Text: "UI Mockup"
  - Text color: RGB: 0, 0, 0

**7. Sound**

- Add a new audio layer with the following settings:
  - Audio file: "background_music.mp3"
  - Audio volume: 50%

**Reproducing the Recipe in Remotion**

```jsx
import { interpolate, spring } from 'remotion';

const backgroundAnimation = () => {
  const background = new BackgroundLayer({
    color: 'rgb(0, 0, 0)',
  });

  const gradient = new GradientLayer({
    type: 'linear',
    direction: 90,
    stops: [
      { stop: 0, color: 'rgb(0, 0, 0)' },
      { stop: 100, color: 'rgb(255, 255, 255)' },
    ],
    mask: new EllipseMask({
      opacity: 0.5,
    }),
  });

  const text = new TextLayer({
    font: 'Open Sans',
    fontSize: 48,
    text: 'What do I want the viewer to feel in this moment?',
    textColor: 'rgb(255, 255, 255)',
  });

  const textAnimator = new TextAnimator({
    type: 'scale',
    scale: { from: 1, to: 1.5 },
    duration: 5000,
    ease: spring(),
  });

  const motionBlur = new MotionBlur({
    type: 'basic',
    amount: 0.5,
    duration: 5000,
  });

  const glow = new Glow({
    type: 'basic',
    color: 'rgb(255, 255, 255)',
    size: 10,
    opacity: 0.5,
  });

  const transition = new Transition({
    type: 'fade',
    duration: 2000,
  });

  return (
    <div>
      {background}
      {gradient}
      {text}
      {textAnimator}
      {motionBlur}
      {glow}
      {transition}
    </div>
  );
};

const uiMockup = () => {
  const composition = new Composition({
    size: { width: 1920, height: 1080 },
    frameRate: 30,
  });

  const solid = new SolidLayer({
    size: { width: 1920, height: 1080 },
    color: 'rgb(255, 255, 255)',
  });

  const text = new TextLayer({
    font: 'Open Sans',
    fontSize: 24,
    text: 'UI Mockup',
    textColor: 'rgb(0, 0, 0)',
  });

  return (
    <div>
      {solid}
      {text}
    </div>
  );
};

const sound = () => {
  const

**Recipe for the After Effects SaaS Tutorial**

**Text Animator Setup:**

1. Create a new text layer in After Effects.
2. Set the font to "Montserrat" and the font size to 24 points.
3. Set the text color to #333333.
4. Create a new text animator by going to "Layer" > "New" > "Text Animator".
5. Select the text layer and click on the "Text Animator" button.
6. Set the animator to "Scale" and set the scale to 100% at frame 0 and 200% at frame 100.
7. Set the easing to "Ease Out" and the duration to 100 frames.

**Masks:**

1. Create a new solid layer in After Effects.
2. Set the layer to "Rectangle" and set the size to 1920x1080.
3. Create a new mask by going to "Layer" > "New" > "Mask".
4. Select the solid layer and click on the "Mask" button.
5. Set the mask to "Rectangle" and set the size to 1920x1080.
6. Set the mask to "Inside" and the feather to 10 pixels.

**Camera/Null Moves:**

1. Create a new null layer in After Effects.
2. Set the null layer to "Position" and set the position to (0, 0).
3. Create a new camera layer in After Effects.
4. Set the camera layer to "Position" and set the position to (0, 0).
5. Set the camera layer to "Rotation" and set the rotation to 0 degrees.
6. Set the camera layer to "Zoom" and set the zoom to 1.

**Motion Blur:**

1. Go to "Composition" > "Composition Settings".
2. Set the motion blur to "On" and the blur amount to 50%.
3. Set the blur duration to 100 frames.

**Glow:**

1. Create a new solid layer in After Effects.
2. Set the layer to "Rectangle" and set the size to 1920x1080.
3. Set the layer to "Color" and set the color to #FFFFFF.
4. Set the layer to "Glow" and set the glow amount to 50%.
5. Set the glow duration to 100 frames.

**Transitions:**

1. Go to "Composition" > "Composition Settings".
2. Set the transition to "Fade In" and the duration to 100 frames.
3. Set the transition to "Fade Out" and the duration to 100 frames.

**UI Mockup Handling:**

1. Create a new solid layer in After Effects.
2. Set the layer to "Rectangle" and set the size to 1920x1080.
3. Set the layer to "Color" and set the color to #333333.
4. Set the layer to "Opacity" and set the opacity to 50%.
5. Set the layer to "Position" and set the position to (0, 0).

**Typography Sizes/Fonts:**

1. Set the font to "Montserrat" and the font size to 24 points.
2. Set the text color to #333333.

**Background Animation:**

1. Create a new solid layer in After Effects.
2. Set the layer to "Rectangle" and set the size to 1920x1080.
3. Set the layer to "Color" and set the color to #FFFFFF.
4. Set the layer to "Opacity" and set the opacity to 50%.
5. Set the layer to "Position" and set the position to (0, 0).
6. Set the layer to "Rotation" and set the rotation to 0 degrees.
7. Set the layer to "Zoom" and set the zoom to 1.

**Sound:**

1. Import a sound file into After Effects.
2. Set the sound file to "Audio" and set the audio to "On".
3. Set the sound file to "Volume" and set the volume to 50%.

**Reproducing the Recipe in Remotion**

**Code-Level Recipe:**

```javascript
import { interpolate, spring } from 'remotion';

const textAnimator = {
  scale: spring(1, {
    fps: 60,
    mass: 1,
    tension: 300,
    friction: 30,
  }),
};

const mask = {
  rectangle: {
    x: 0,
    y: 0,
    width: 1920,
    height: 1080,
  },
  inside: true,
  feather: 10,
};

const camera = {
  position: {
    x: 0,
    y: 0,
  },
  rotation: {
    x: 0,
    y: 0,
    z: 0,
  },
  zoom: 1,
};

const motionBlur = {
  on: true,
  blurAmount: 50,
  blurDuration: 100,
};

const glow = {
  on: true,
  glowAmount: 50,
  glowDuration: 100,
};

const transition = {
  fadeIn: {
    duration: 100,
  },
  fadeOut: {
    duration: 100,
  },
};

const
