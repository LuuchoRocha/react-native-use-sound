# react-native-use-sound

### 🔊 A React Native Hook for playing sounds 🔊

react-native-use-sound is largely based on the work by @joshwcomeau **[use-sound](https://github.com/joshwcomeau/use-sound)**

## Installation

Package can be added using **yarn**:

```bash
yarn add react-native-use-sound
cd ios && pod install
```

Or, use NPM:

```bash
npm install react-native-use-sound
cd ios && pod install
```

## Examples

### Basic Example

```js
import useSound from "react-native-use-sound";

const BoopButton = () => {
  const boopSfx =
    "http://commondatastorage.googleapis.com/codeskulptor-demos/DDR_assets/Kangaroo_MusiQue_-_The_Neverwritten_Role_Playing_Game.mp3";
  const [play, pause, stop, data] = useSound(boopSfx);

  const handlePlay = () => {
    if (!data.isPlaying) play();
    else pause();
  };

  return <Button onPress={handlePlay}>Boop!</Button>;
};
```

---

## API Documentation

See the **[use-sound](https://github.com/joshwcomeau/use-sound)** documentation.
