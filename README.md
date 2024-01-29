# Introduction
The useGamepad React Hook is designed for seamless integration of game controller support in
React applications. It provides an easy-to-use API to access gamepad inputs like buttons and
joysticks, enhancing the interactivity of your web app.

## Installation Instructions
1. Add the useGamepad.jsx file to your project's components directory.
2. Import the useGamepad hook in your React component using ES6 syntax:
 `import { useGamepad } from './useGamepad';`
## Usage Guide
In your React component, use the hook as follows:
```
const { buttonA, buttonB, buttonX, buttonY, joystick, joystickRight, LB, RB, RT, LT, up, down, left, right, start, select } = useGamepad();
```
This will give you access to the gamepad's buttons and joysticks.
You can as well choose to get only the buttons you want.

## API Reference
The useGamepad hook provides the following properties:
- buttonA, buttonB, buttonX, buttonY: Boolean states of the A, B, X, Y buttons.
- joystick, joystickRight: Object states of the left and right joysticks.
- LB, RB, RT, LT: States of the left and right bumpers and triggers.
- up, down, left, right: States of the directional pad.
useGamepad React Hook Documentation
- start, select: States of the start and select buttons.
## Example
Here is a simple example of using the useGamepad hook in a component:
```
import React from 'react';
import { useGamepad } from './useGamepad';
function GameComponent() {
 const { buttonA } = useGamepad();
 return (<div>{buttonA ? 'Button A Pressed' : 'Press Button A'}</div>);
}
export default GameComponent;
```
## FAQs
Q: How do I handle multiple gamepads?
A: The hook is designed to handle multiple gamepads. You can access them using array indexes.
Q: Is this hook compatible with all browsers?
A: The hook uses the standard Gamepad API, which is widely supported in modern browsers.
## Contact Information
For support or contributions, please visit the project repository on GitHub or contact the maintainers.