# react-native-begin-background-task

## Installation

### Mostly automatic installation

1. Add this to your dependencies in `package.json`: `"react-native-begin-background-task": "git+https://github.com/blockfirm/react-native-begin-background-task.git"`
2. Run `npm install`
3. **React Native 0.60+**: `$ cd ios && pod install`  
   **React Native <0.60**: `$ react-native link react-native-begin-background-task`

### Manual installation

1. Add this to your dependencies in `package.json`: `"react-native-begin-background-task": "git+https://github.com/blockfirm/react-native-begin-background-task.git"`
2. Run `npm install`
3. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
4. Go to `node_modules` ➜ `react-native-begin-background-task` and add `RNBeginBackgroundTask.xcodeproj`
5. In XCode, in the project navigator, select your project. Add `libRNBeginBackgroundTask.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
6. Run your project (`Cmd+R`)

## Usage

```javascript
import { beginBackgroundTask, endBackgroundTask } from 'react-native-begin-background-task';

// ...
const backgroundTaskId = await beginBackgroundTask();
// ...
await endBackgroundTask(backgroundTaskId)
```
