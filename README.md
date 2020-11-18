# react-native-loading-animation-image
React Native Loading Animation Image component for both Ios and Android

## Add it to your project

1. Insall package
    - Using NPM
    `npm i -S react-native-loading-animation-image` 
    - Using Yarn
    `yarn add react-native-loading-animation-image`
2. Import package
    `import { LoadingAnimation  } from 'react-native-loading-animation-image';`

## Usage



```javascript
import React from 'react';
import { LoadingAnimation  } from 'react-native-loading-animation-image';
class App extends React.Component  {
    state = {
        isLoading: true
    }

    render() {
        return (
            <View style={{flex: 1}}>
                <LoadingAnimation 
                visible={this.state.isLoading} 
                source={{uri: 'https://avatars0.githubusercontent.com/u/42457760?s=400&u=0b50aa5f00553d1041794c622e22139aa8c7d7e6&v=4'}}
                />
            </View>
        );
    }
}
```


## Props

- **`visible`** _(Boolean)_ - The visible prop determines whether your modal is visible.
- **`source`** _(String)_  * `uri` is a string representing the resource identifier for the image, which
     * could be an http address, a local file path, or the name of a static image
     * resource (which should be wrapped in the `require('./path/to/image.png')`
     * function).

**MIT Licensed**
