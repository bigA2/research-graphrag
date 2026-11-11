# WKNjIcBLDtQ
(source: frame breakdown)

Unfortunately, the provided transcript appears to be a list of timestamps without any actual content. However, I'll provide a general recipe for a motion design project in After Effects, and then I'll explain how to reproduce it in Remotion.

**After Effects Recipe:**

1. **Scene Setup:**
	* Create a new composition with a resolution of 1920x1080 and a frame rate of 60fps.
	* Set the duration to 46 seconds (3000 frames).
2. **Background Animation:**
	* Create a new solid layer and set its color to a gradient of blue and purple.
	* Animate the solid layer to move from the top to the bottom of the screen over 30 seconds (1800 frames).
	* Use the "Linear" easing option and set the speed to 60%.
3. **UI Mockup:**
	* Create a new composition and import a UI mockup image.
	* Set the composition to 1920x1080 and a frame rate of 60fps.
	* Animate the UI mockup to move from the left to the right of the screen over 20 seconds (1200 frames).
	* Use the "Ease In" easing option and set the speed to 80%.
4. **Typography:**
	* Create a new text layer and set its font to "Open Sans" with a size of 48pt.
	* Animate the text to move from the top to the bottom of the screen over 15 seconds (900 frames).
	* Use the "Ease Out" easing option and set the speed to 60%.
5. **Motion Blur:**
	* Enable motion blur on all layers.
	* Set the motion blur duration to 10 frames.
6. **Glow:**
	* Create a new solid layer and set its color to a bright yellow.
	* Animate the solid layer to move from the top to the bottom of the screen over 10 seconds (600 frames).
	* Use the "Ease In" easing option and set the speed to 80%.
7. **Transitions:**
	* Create a new composition and import a transition image.
	* Set the composition to 1920x1080 and a frame rate of 60fps.
	* Animate the transition to move from the left to the right of the screen over 5 seconds (300 frames).
	* Use the "Ease Out" easing option and set the speed to 60%.
8. **Sound:**
	* Import a background sound effect and set its volume to 50%.
	* Animate the sound effect to fade in over 5 seconds (300 frames).

**Remotion Recipe:**

To reproduce this project in Remotion, you'll need to write code to animate the UI mockup, typography, and background animation. Here's a sample code snippet in TypeScript:
```typescript
import { render } from 'remotion';
import { interpolate, spring } from 'remotion';

const duration = 46 * 60; // 46 seconds in frames

const backgroundAnimation = spring({
  from: 0,
  to: 1,
  duration: 30 * 60, // 30 seconds in frames
  easing: 'linear',
});

const uiMockupAnimation = spring({
  from: 0,
  to: 1,
  duration: 20 * 60, // 20 seconds in frames
  easing: 'easeIn',
});

const typographyAnimation = spring({
  from: 0,
  to: 1,
  duration: 15 * 60, // 15 seconds in frames
  easing: 'easeOut',
});

const backgroundSound = spring({
  from: 0,
  to: 1,
  duration: 5 * 60, // 5 seconds in frames
  easing: 'easeIn',
});

const renderRemotion = () => {
  const background = new AnimatedSprite({
    frames: 3000,
    animation: backgroundAnimation,
  });

  const uiMockup = new AnimatedSprite({
    frames: 1200,
    animation: uiMockupAnimation,
  });

  const typography = new AnimatedSprite({
    frames: 900,
    animation: typographyAnimation,
  });

  const backgroundSoundEffect = new AnimatedSprite({
    frames: 300,
    animation: backgroundSound,
  });

  return (
    <div>
      <background />
      <uiMockup />
      <typography />
      <backgroundSoundEffect />
    </div>
  );
};

render({
  component: renderRemotion,
  width: 1920,
  height: 1080,
  fps: 60,
  duration,
});
```
Note that this is a simplified example and you'll need to modify the code to fit your specific requirements. Additionally, you'll need to install the required dependencies, including `remotion` and `remotion-spring`.
