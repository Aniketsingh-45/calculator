# 🧮 Glassmorphic Calculator — Modern Web Calculator

A lightweight, responsive, and aesthetically striking web-based calculator. Designed with a sleek dark-themed glassmorphism UI, interactive text background animations, and custom responsive layouts for mobile, tablet, and desktop screens.

Built entirely using native Web technologies: **HTML5**, **Vanilla CSS3**, and **Vanilla JavaScript**—zero external frameworks, zero dependencies, and extremely fast rendering performance.

---

## 🌟 Key Features

*   **Premium Glassmorphic Design**: Features a semi-transparent dark container with soft outer glows, subtle borders, and smooth button hover micro-animations.
*   **Dynamic Animated Title**: The "MY CALCULATOR" heading features an animated background texture clipped to text, providing a premium visual feel on load.
*   **Fully Responsive Layout**: Integrated media queries adjust container sizing, input padding, button dimensions, and fonts automatically for different screen widths down to 320px (mobile-friendly).
*   **Vanilla JS Computation Engine**: Calculates inputs dynamically using basic event delegation and JavaScript evaluations, supporting key clearing (`AC`) and character deletion (`DEL`).
*   **Accented Keyboards**: Uses dedicated accent colors for special function keys (green for `AC`, `DEL`, `%`, `/`, `*`, `-`, `+`) and a bright, custom hover state for the equals button (`=`).

---

## 🛠️ File Structure

The project has a clean and simple structure:

*   [calculator.html](file:///d:/My%20Apps/project/calculator/calculator.html): Defines the markup structure, including the display input and the grid representation of numbers and operators.
*   [style.css](file:///d:/My%20Apps/project/calculator/style.css): Custom stylesheet incorporating imported Google Fonts (`Poppins`), layouts, keyframe animation rules, and screen-size media breakpoints.
*   [script.js](file:///d:/My%20Apps/project/calculator/script.js): Handles button clicks, UI state updates, mathematical evaluations, and clearing logic.

---

## 💻 Tech Stack & Design Choices

*   **Structure**: Semantic HTML5 layout defining input components and grouped interactive buttons.
*   **Typography**: Integrated Google Fonts including `Poppins`, `Alumni Sans SC`, `Dancing Script`, and `Source Code Pro` for clean, readable numbers and letters.
*   **Styling & Themes**:
    *   **Linear Gradients**: Uses a smooth diagonal background gradient (`45deg, black, rgb(76, 89, 102)`).
    *   **Glassmorphism**: Combines `transparent` backgrounds, `box-shadow` overlays, and subtle solid borders (`1px solid gray`).
*   **Micro-Animations**:
    *   **Header Animation**: The header uses a background image clipped to text moving via keyframe animation to create a glittering effect:
        ```css
        @keyframes animate {
            to {
                background-position-x: 500px;
            }
        }
        ```
    *   **Interactive Hover States**: Standard buttons smoothly transitions on hover via opacity offsets, while the equals button (`.equalBtn`) changes background to a darker hue.
*   **Calculation Logic**: Implemented using basic query selectors and a loop mapping click events to execute calculations:
    ```javascript
    arr.forEach(button => {
        button.addEventListener('click', (e) => {
            if (e.target.innerHTML == "=") {
                string = eval(string);
                input.value = string;
            }
            // AC & DEL operations
        })
    })
    ```

---

## 🚀 How to Run

1.  Clone or download this project directory onto your machine.
2.  Navigate to the directory: `d:\My Apps\project\calculator`.
3.  Open the [calculator.html](file:///d:/My%20Apps/project/calculator/calculator.html) file directly in any modern web browser (Google Chrome, Mozilla Firefox, Safari, Microsoft Edge, Brave, etc.) by double-clicking it.
4.  No development servers, build configurations, or node packages are required!
