# 🎭 Personality Quiz Game (لعبة الشخصيات)

This is a simple personality quiz built with HTML, CSS, and JavaScript, designed for Arabic-speaking users. The game consists of 10 questions answered using range sliders, and based on the responses, it determines the character that best fits the user's personality.

## 🚀 Features

- Fully responsive and RTL (right-to-left) layout for Arabic.
- Smooth, interactive range sliders with custom-colored tracks:
  - The filled portion of the slider (from start to current value) is colored **blue**.
  - The remaining portion is colored **light gray**.
- Animated reveal of the result with character matching logic.
- Clean, minimalistic design using the Cairo font.

## 🎨 Range Slider Customization

The range sliders are customized using:

- CSS `linear-gradient` to visually represent the selected value.
- JavaScript to update the background dynamically on user input.

### Example:

If a slider value is `2` out of `5`, 40% of the slider will be blue, and the remaining 60% will be gray.

```js
const percentage = ((val - min) / (max - min)) * 100;
this.style.background = `linear-gradient(to right, #007bff 0%, #007bff ${percentage}%, #ddd ${percentage}%, #ddd 100%)`;
