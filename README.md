# AutoResizingInput Component

![GitHub release](https://img.shields.io/github/release/codeMigue/expo-auto-resizing-input.svg)  
[Check the Releases](https://github.com/codeMigue/expo-auto-resizing-input/releases)

Welcome to the AutoResizingInput Component! This React Native component allows you to create an auto-resizing text input that expands as you type. It mimics the behavior of modern messaging apps like iMessage and WhatsApp, offering a smooth and engaging user experience.

## Table of Contents

- [Features](#features)
- [Platform Support](#platform-support)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Features

- 🚀 **Auto-resizing**: The input container grows upward as you type multiple lines, ensuring your content is always visible.
- 🎬 **Smooth animations**: Built with React Native Reanimated, the component delivers 60fps performance for a fluid experience.
- 📱 **Cross-platform**: Enjoy full functionality on iOS, Android, and Web platforms.
- 🎯 **Send button**: The adaptive send button changes color based on the input state, providing visual feedback.
- 🔧 **Action icons**: Four customizable action buttons (attach, rocket, magic, science) let you tailor the component to your needs.
- ⌨️ **Keyboard shortcuts**: Use Enter to send messages and Shift+Enter for a new line on the Web.
- 🎨 **Modern UI**: The component features a dark theme styled with Tailwind CSS, giving it a contemporary look.
- 📝 **TypeScript**: Fully typed with TypeScript support, ensuring type safety and better development experience.

## Platform Support

| Platform  | Status         | Notes                               |
|-----------|----------------|-------------------------------------|
| **iOS**   | ✅ Full Support | Native animations, keyboard handling |
| **Android**| ✅ Full Support | Native animations, keyboard handling |
| **Web**   | ✅ Full Support | Keyboard shortcuts available         |

## Installation

To get started with the AutoResizingInput component, you can install it using npm or yarn. Here’s how:

### Using npm

```bash
npm install expo-auto-resizing-input
```

### Using yarn

```bash
yarn add expo-auto-resizing-input
```

## Usage

After installing the component, you can import and use it in your React Native project. Here’s a simple example:

```javascript
import React, { useState } from 'react';
import { View } from 'react-native';
import AutoResizingInput from 'expo-auto-resizing-input';

const App = () => {
  const [text, setText] = useState('');

  return (
    <View style={{ padding: 20 }}>
      <AutoResizingInput
        value={text}
        onChangeText={setText}
        placeholder="Type your message..."
      />
    </View>
  );
};

export default App;
```

This code creates a basic application with an auto-resizing input. As you type, the input will grow, providing a seamless experience.

## Customization

The AutoResizingInput component offers various customization options to fit your design needs. You can change styles, placeholder text, and button actions. Here are some common customization options:

### Styling

You can customize the styles of the input and buttons by passing style props:

```javascript
<AutoResizingInput
  style={{ borderColor: 'gray', borderWidth: 1, borderRadius: 5 }}
  sendButtonStyle={{ backgroundColor: 'blue' }}
/>
```

### Placeholder Text

Change the placeholder text to guide users on what to type:

```javascript
<AutoResizingInput
  placeholder="Type your message here..."
/>
```

### Action Buttons

You can customize the action buttons by providing your own icons or changing their behavior:

```javascript
<AutoResizingInput
  actionButtons={[
    { icon: 'attach', onPress: () => console.log('Attach pressed') },
    { icon: 'rocket', onPress: () => console.log('Rocket pressed') },
  ]}
/>
```

## Contributing

We welcome contributions to improve the AutoResizingInput component. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with clear messages.
4. Push your branch to your forked repository.
5. Create a pull request describing your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Additional Resources

For more information on how to use React Native, you can visit the [official React Native documentation](https://reactnative.dev/docs/getting-started). 

For updates and new releases, [check the Releases section](https://github.com/codeMigue/expo-auto-resizing-input/releases).

Feel free to reach out if you have any questions or suggestions. Happy coding!