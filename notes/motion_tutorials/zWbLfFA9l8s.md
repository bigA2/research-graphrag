# zWbLfFA9l8s
(source: transcript)

**Recipe for the SaaS Animation Style**

**Background Animation**

1. Create a new solid layer and add a gradient ramp.
2. Set the bottom color to a light gray and the top color to a darker gray.
3. Create a new shape layer and draw a shape using the pen tool.
4. Disable the stroke and set the fill to a light purple.
5. Duplicate the shape layer and drag it backwards, setting the color to an even lighter purple.
6. Duplicate the shape layer again and set the color to a darker purple.
7. Precompose the shape layers and add a Gaussian blur with an amount of 350.
8. Set the opacity to 50% and duplicate the precomposed layer.
9. Add a transform effect and set the scale height to 100 and the width to minus 100.
10. Add a hue and saturation effect and play with the master hue to change the color.
11. Decrease the layer's opacity to 30%.
12. Add a turbulent displace effect and keyframe the evolution to four.
13. Copy the turbulent displace effect and paste it on the precomposed layer above, dragging the keyframe back.

**Text Animation**

1. Create a new text layer and write out the word "this".
2. Set the font type to medium and click on animate and position.
3. Drop down the position and expand the advanced tab.
4. Set the based on function to words and the shape to ramp up and the units to index.
5. Keyframe the end and move it to the beginning, setting the end to five.
6. Add a blur property and set it to 10.
7. Add an opacity property and set it to 30.
8. Add a fill color property and set the color to purple.
9. Duplicate the text and write out "is".
10. Move the duplicated text to the right and delete the layer.
11. Create a new null object and parent the text layer to it.
12. Keyframe the position at the beginning and turn on the grid.
13. Move the layers to the left and select the keyframes.
14. Go into the speed graph and start it slow and end it slow.
15. Move the keyframes even more to the left and select them again.
16. Do the same to the graph again.

**Icon Animation**

1. Create a new shape layer and select the rectangle tool.
2. Draw a rectangle and center it to the middle.
3. Change the color to white and set the roundness to 60.
4. Set the scale to 80 and drag in the Ultimate Editor's logo.
5. Track matte the logo to the shape layer and duplicate the shape layer.
6. Drag the duplicated shape layer below the logo layer.
7. Enable the view, enable the stroke, and set the stroke color to white.

**Transition**

1. Create a new shape layer and draw a shape using the pen tool.
2. Disable the stroke and set the fill to a light purple.
3. Duplicate the shape layer and drag it backwards, setting the color to an even lighter purple.
4. Duplicate the shape layer again and set the color to a darker purple.
5. Precompose the shape layers and add a Gaussian blur with an amount of 350.
6. Set the opacity to 50% and duplicate the precomposed layer.
7. Add a transform effect and set the scale height to 100 and the width to minus 100.
8. Add a hue and saturation effect and play with the master hue to change the color.
9. Decrease the layer's opacity to 30%.
10. Add a turbulent displace effect and keyframe the evolution to four.
11. Copy the turbulent displace effect and paste it on the precomposed layer above, dragging the keyframe back.

**Reproducing in Remotion**

To reproduce this animation in Remotion, you would need to write code to achieve the same effects. Here's a possible implementation:

```jsx
import { spring } from 'remotion';

const background = () => {
  const gradient = spring(0.5, { damping: 100 });
  const purple = spring(0.3, { damping: 100 });
  const darkerPurple = spring(0.2, { damping: 100 });

  return (
    <div
      style={{
        position: 'absolute',
        top: 0,
        left: 0,
        width: '100%',
        height: '100%',
        background: `linear-gradient(to bottom, ${purple} 0%, ${darkerPurple} 100%)`,
      }}
    />
  );
};

const text = () => {
  const thisText = spring(0.5, { damping: 100 });
  const isText = spring(0.3, { damping: 100 });

  return (
    <div
      style={{
        position: 'absolute',
        top: 0,
        left: 0,
        width: '100%',
        height: '100%',
        fontSize: 24,
        color: 'purple',
        textShadow: '0 0 10px #fff',
      }}
    >
      <span style={{ opacity: thisText }}>{'this'}</span>
      <span style={{ opacity: isText, marginLeft: 20 }}>{'is'}</span>

**Recipe for the Animation:**

1. **Stroke Color and Increase:**
	* Set the stroke color to white
	* Increase the stroke size to 10px
2. **Drop Shadow:**
	* Add a drop shadow on the shape layer
	* Set the distance to 17
	* Set the softness to 40
	* Set the opacity to 25
3. **Inner Glow:**
	* Add an inner glow on the UE logo
	* Set the color to white
	* Set the size to 90
	* Decrease the opacity to 21
4. **Parenting and Scaling:**
	* Parent the UE icon and the shape layer below to the other shape layer
	* Scale it down and place it like so
	* Rotate it, keyframe the scale, rotation, and position
5. **Bounce Effect:**
	* Click on bounce it for position, scale, and rotation
6. **Text Layer:**
	* Duplicate the text layer
	* Move the layer over here
	* Change the text to 2.0
	* Move it to the right
	* Change the font type to heavy
7. **Shape Layer:**
	* Add a shape layer
	* Move it to where the text starts
	* Create a square using the rectangle tool
	* Decrease the stroke
	* Move the shape layer under the text
	* Increase the roundness all the way up
	* Center the anchor point and scale it up
	* Add a four color gradient on it
	* Set the blend to 25
	* Change the colors to white and a light purple
	* Add a gradient ramp on the 2.0 text layer
	* Adjust the points like so
	* Change the first color to a dark purple and the second one to a lighter purple
	* Parent the shape layer to the null layer
8. **Keyframe Animation:**
	* Keyframe the scale and rotation
	* Move back and start the scale at zero and increase the rotation to minus 14
	* Press bounce it for rotation and then select scale and bounce it again
9. **Duplicate and Scale:**
	* Duplicate the shape layer
	* Move the layer down
	* Delete the bouncer effect on the foreground gradient
	* Go to the last keyframe and scale it up
	* Change the color to a light pink
10. **Transition:**
	* Keyframe the scale for the shape layer
	* Move forward and increase it until you fill the screen up
	* Select the keyframes and go into the speed graph
	* Start it slow and end it fast
	* Cut the layers below like this
	* Keyframe the scale for the 2.0 text
	* Move forward and increase it to 110
	* Move forward again and set it to zero
	* Then just bounce the scale
	* Select the keyframes and go into the speed graph
	* Copy my graph
	* For the shape layer, keyframe the opacity
	* Move forward and set it to zero

**Reproducing the Animation in Remotion:**

To reproduce the animation in Remotion, you would need to write code that achieves the same effects as the After Effects animation. Here's a possible implementation:

```jsx
import { spring } from 'remotion';

const animation = () => {
  const strokeColor = 'white';
  const strokeSize = 10;
  const dropShadowDistance = 17;
  const dropShadowSoftness = 40;
  const dropShadowOpacity = 25;
  const innerGlowColor = 'white';
  const innerGlowSize = 90;
  const innerGlowOpacity = 21;
  const textLayerText = '2.0';
  const textLayerFont = 'heavy';
  const shapeLayerRoundness = 100;
  const shapeLayerStroke = 0;
  const shapeLayerGradientColors = ['white', 'lightPurple'];
  const shapeLayerGradientBlend = 25;
  const shapeLayerScale = 0;
  const shapeLayerRotation = -14;
  const shapeLayerOpacity = 0;
  const transitionScale = 110;
  const transitionOpacity = 0;

  const springConfig = {
    stiffness: 100,
    damping: 20,
  };

  const animation = () => {
    const time = useCurrentFrame();

    const stroke = spring(strokeSize, springConfig);
    const dropShadow = spring(dropShadowOpacity, springConfig);
    const innerGlow = spring(innerGlowOpacity, springConfig);
    const textLayerScale = spring(transitionScale, springConfig);
    const textLayerOpacity = spring(transitionOpacity, springConfig);
    const shapeLayerScale = spring(shapeLayerScale, springConfig);
    const shapeLayerRotation = spring(shapeLayerRotation, springConfig);
    const shapeLayerOpacity = spring(shapeLayerOpacity, springConfig);

    return (
      <div>
        <svg
          width="100%"
          height="100%"
          viewBox="0 0 100 100"
          fill="none"
          xmlns="http://www.w3.org/2000/svg

**Recipe for the Animation:**

1. **UE Logo:**
	* Create a new shape layer and draw a square with a roundness of 88.
	* Set the fill to a gradient with white and light pink colors.
	* Increase the stroke to 20 pixels and add a drop shadow with a distance of 15, softness of 45, and opacity of 7.
	* Create a new text layer and write out "UE" with a font type of black.
	* Decrease the pacing and scale it up, align it, and add a four-color gradient.
	* Adjust the gradient points and colors to match the logo.
	* Add a CC light sweep and set the intensity to zero, angle to the left, and edge thickness to 3.
	* Add a Deep Glow with a threshold mode of luminance, threshold of 82, and exposure of 0.5.
2. **Glass Design:**
	* Create a new shape layer and draw a stretched rectangle.
	* Go into the gradient editor and add a bunch of colors.
	* Play with the color variation and stick to the same light color scheme.
	* Drag the gradient points and set the stroke to 10 pixels.
	* Duplicate the shape layer and add a flip effect.
	* Add a linear wipe effect with an angle of minus 90, completion of 60, and feather of 95.
	* Copy the linear wipe and paste it on the other shape layer, changing the angle and opacity.
	* Select the rectangle tool and draw a rectangle, center it, and increase the roundness.
	* Go into the gradient editor and delete the points, but keep the two over here.
	* Change the last two colors to a light purple and adjust the gradient points.
	* Disable the stroke and duplicate the UI text layer, bringing it up and setting the parents to none.
	* Change the text to "fastest" and scale it down, moving it up.
	* Adjust the four-color gradient points from the text layer and add them to the icon.
	* Move the icon over here, copy the effects from the text layer, and paste them onto the icon.
	* Adjust the gradient points and play with the colors until you end up with this.
3. **Glass UI:**
	* Duplicate the placeholder glass UI shape layer and bring it up.
	* Set the gradient ramp to fill and change the color to black.
	* Right-click and add an inner glow, expanding the tab and setting the color to white and increasing the size.
	* Create an adjustment layer and drag a Gaussian blur on it, setting the blurriness to 100 and tracking matte it to the shape layer.
	* Click on the little icon and track matte the icon to the shape layer, enabling the layer back.
	* Drag a brightness and contrast onto the adjustment layer and decrease the brightness.
	* Add a displacement map on the adjustment layer, setting the displacement map to the shape layer.

**Reproducing the Animation in Remotion:**

To reproduce the animation in Remotion, you can use the following code:

```javascript
import { interpolate, spring } from 'remotion';

const logo = {
  x: 0,
  y: 0,
  scale: 1,
  rotation: 0,
  opacity: 1,
};

const glass = {
  x: 0,
  y: 0,
  scale: 1,
  rotation: 0,
  opacity: 1,
};

const animation = () => {
  const time = useCurrentTime();

  const logoX = interpolate(time, [0, 100], [0, 100], {
    easing: spring(),
  });

  const logoY = interpolate(time, [0, 100], [0, 100], {
    easing: spring(),
  });

  const logoScale = interpolate(time, [0, 100], [1, 2], {
    easing: spring(),
  });

  const logoRotation = interpolate(time, [0, 100], [0, 360], {
    easing: spring(),
  });

  const logoOpacity = interpolate(time, [0, 100], [1, 0], {
    easing: spring(),
  });

  const glassX = interpolate(time, [0, 100], [0, 100], {
    easing: spring(),
  });

  const glassY = interpolate(time, [0, 100], [0, 100], {
    easing: spring(),
  });

  const glassScale = interpolate(time, [0, 100], [1, 2], {
    easing: spring(),
  });

  const glassRotation = interpolate(time, [0, 100], [0, 360], {
    easing: spring(),
  });

  const glassOpacity = interpolate(time, [0, 100], [1, 0], {
    easing: spring(),
  });

  return (
    <div>
      <div
        style={{
          position: 'absolute',
          left: logoX,
          top: logoY,
          transform: `scale(${logoScale}) rotate(${logoRotation}deg)`,
          opacity: logoOpacity,
        }}
      >
        <img src="logo.png" />
      </div>
      <div
        style

**Recipe for the After Effects Animation:**

1. **Displacement Map**
	* Add a displacement map to the shape layer below.
	* Set the horizontal displacement to -30.
	* Set the vertical displacement to -30.
2. **Adjustment Layer**
	* Add a transform effect to the adjustment layer.
	* Set the scale to 120.
	* Move the layer above the displacement map.
3. **Duplicate Layer**
	* Duplicate the layer above the displacement map.
4. **Text Animation**
	* Delete the light sweep and deep glow effects from the fastest text.
	* Scale the text and move it up.
	* Track matte the text to the shape layer.
	* Set the opacity keyframe to 25.
	* Add a gradient ramp to the text.
	* Duplicate the gradient points.
	* Adjust the four-color gradient points.
5. **Icon Animation**
	* Duplicate the icon.
	* Move the icon to the right.
	* Delete all effects from the icon.
	* Add a gradient ramp to the icon.
	* Adjust the points of the gradient ramp.
	* Decrease the opacity of the icon.
	* Scale the icon up and adjust its position.
6. **UI Layers**
	* Select all UI layers.
	* Duplicate the UI layers.
	* Bring the duplicated layers up.
	* Move the position of the duplicated layers to the right.
	* Delete the layers like so.
7. **Text and Shadow Animation**
	* Change the main text to "easiest".
	* Adjust the four-color gradient points.
	* Play with the colors until you end up with this.
8. **Icon and Placeholder Animation**
	* Drag the icon below the adjustment layer.
	* Change the position of the icon like so.
	* Copy all effects from the lighting icon.
	* Paste the effects on the hand icon.
	* Delete the lighting icon.
	* Track matte the hand icon into the placeholder.
	* Play with the colors until you end up with this.
9. **Light Sweep Animation**
	* Set the light sweep to the center.
	* Change the direction to the center.
	* Duplicate the hand icon.
	* Delete all effects from the duplicated hand icon.
	* Move the duplicated hand icon to the right.
	* Copy the gradient ramp from the lighting shadow layer.
	* Paste the gradient ramp on the hand icon.
	* Delete the lightning shadow.
	* Set the blending mode to darken.
	* Change the gradient ramp to this orange.
	* Set the opacity to 30.
10. **Text Easiest Animation**
	* Set the light sweep to the center.
	* Duplicate the text easiest.
	* Move the duplicated text easiest to the right.
	* Delete the light sweep and deep glow effects from the duplicated text easiest.
	* Scale the duplicated text easiest.
	* Move the duplicated text easiest up.
11. **UI Glass Animation**
	* Push the UI glass layers to the right.
	* Keyframe the transition completion for the gradient layers.
	* Move the keyframes back and start them at 100.
	* Select the keyframes and go into the speed graph.
	* Start the keyframes fast and end them slow.
	* Delay the layers.
12. **Icon and Shadow Animation**
	* Select the first UI layers.
	* Drag them over to the first UI layers.
	* Select the icon and the icon's shadow.
	* Keyframe the position of the icon and the shadow.
	* Move the keyframes back and start the shadow to the right.
	* Move the icon to the left.
	* Bounce the icon and the shadow.
	* Keyframe the scale for the text shadow.
	* Move the keyframes forward and start the shadow by scaling it down.
	* Bounce the shadow.
	* Keyframe the position of the placeholder.
	* Move the keyframes forward and start the placeholder at the left.
	* Bounce the placeholder.
	* Keyframe the rotation of the placeholder.
	* Move the keyframes forward and rotate the placeholder like so.
	* Bounce the rotation keyframes.
	* Delay the layers.
13. **Transition Animation**
	* Select the two text layers.
	* Duplicate the text layers.
	* Bring the duplicated text layers over.
	* Change the text to "2026".
	* Change the font type to black.
	* Align the text in the middle.
	* Create a new shape layer.
	* Draw a big circle like so.
	* Center the circle and change the gradient fill.
	* Set the color to a slight purple.
	* Keyframe the scale and increase it until you fill up the whole screen.
	* Go back and start it at zero.
	* Select the keyframes and start them slow and end them fast.
	* Track mat the shape layer to the 2026 text layer.
	* Enable the layer.
	* Duplicate the shape layer again.
	* Delay the duplicated shape layer.
	* Change the color to a lighter pink.
	* Duplicate the shape layer again.
	* Delay the duplicated shape layer.
	* Change the color to an even lighter pink.
	* Remove the track mat.
	* Duplicate the shape layer again.
	* Delay
