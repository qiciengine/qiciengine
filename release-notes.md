# Release Notes
Downloads / New Features / Enhancements / Bug Fixes for QICI Engine

## Examples

A wide range of [source code examples](http://engine.qiciengine.com/demo/) for you to explore. Download all in [one zip](http://engine.qiciengine.com/demo/QICI_Demos.zip) file.   

## 2016-03-04, Version 1.0.8

### Downloads
[QICI Engine v1.0.8](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.8.zip)

### New Features
- Dropdown game object
- TweenTransform Component
- Highlight and locate JavaScript file from Inspector panel
- Resolution Settings

### Enhancements
- Change UIImage and Sprite's texture type from qc.Atlas to qc.Texture
- Add autoHide property on ScrollBar
- Highlight current scene in Project panel
- Enchance Action editor
- Enable/Disable auto refresh in Preference settings
- Disconnectable relation between Node and Prefab
- Enchance WebGL support check, and change WebGL rendering to Auto mode
- Add Undo and Redo features for Tween Curve editing
- Auto apply changes in Project Settings panel

### Bugs Fixes
- Fixed Particle System bug in dirty rectangles management mode
- Fixed getting wrong sound duration issue
- Fixed Particle System Emitter Prefab modify error issue 
- Fixed UIText rendering bug when filtering
- Fixed Filter error when its range exceeds the screen size

## 2016-01-28, Version 1.0.7

### Downloads
[QICI Engine v1.0.7](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.7.zip)

### New Features
- Rich Text plugin
- Particle System plugin (Beta)
- Action editor (Beta)
- Box2D Plugin (Beta) 
- Option to fix game size in project settings

### Enhancements
- Changed 'state' terminology usage to 'scene' throughout QICI
- Changed snapshotAsImage method parameter from global to local 
- Added setTileIndex method (supports modifying tiles) to TileLayer
- Added qc.Des.encrypt and qc.Des.decrypt data encryption methods
- Changed the default duration value of Tween from 0 to 1 
- Improved the Arcade physics scheduling
- Prevent image drawing when width or height is 0 in Canvas rendering mode
- Added onDeserialized event to Node
- Added r, g, b properties to qc.Color
- Added alpha property to qc.Dom
- Enabled roundPixeds in Canvas rendering mode
- Improved the Editor Welcome Page
- Disabled instant delete (via keyboard or menu) for some directories

### Bugs Fixes
- Fixed: children missing update when parent is removed in dirty rectangles management
- Fixed: position update delay of NodeMask componet draw in RenderTexture
- Fixed: qc.Dom bug in [Tencent X5 browser](http://x5.tencent.com/)
- Fixed: Slider's canPurse failure when fixedSize a negative value
- Fixed: Buttons no longer clickable when parent invisible
- Fixed: frameNames error when texture atlas is only one image
- Fixed: InputField on longer editable when parent invisible
- Fixed: Array type serialization bug
- Fixed: maximum frame rate limit not working

## 2016-01-08, Version 1.0.6

### Downloads
[QICI Engine v1.0.6](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.6.zip)

### Enhancements
- Reduce the canvas consumption in Tilemap's layers 
- Improve the process performance for interaction

### News
- Add the funtion to enable or disable antialiasing dynamically
- Add the device information to be displayed in DebugViewer component
- Add addListenerOnce and removeListener methods on Node and Behaviour
- Add the function to run script from the server to the specified client browser

### Bug Fixes
- Fix the callback function parameter loss issue in Arcade Physics
- Fix the dirty rectangles management bug in some components
- Fix the game stuck issue on some mobile browsers when the mp3 file asset is missing
- Fix the scene can not clean clearly issue when enabling dirty rectangles management in editor

## 2016-01-04, Version 1.0.5

### Downloads
[QICI Engine v1.0.5](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.5.zip)

### Enhancements
- Optimize canvas rendering with the management of dirty rectangles 

### News
- Set all Dom's box-sizing css value as border-box in style.css 
- Add the function to call the client to run script from the server 

### Bug Fixes
- Fix the extend editor scripts missing import issue
- Fix the wrong CalcUpdateTransform parameter value in DebugViewer

## 2015-12-31, Version 1.0.4

### Downloads
[QICI Engine v1.0.4](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.4.zip)

### Enhancements
- Significantly improve the rendering performance on [Tencent X5 browser](http://x5.tencent.com/)
- Use the IP address to replace the localhost for the URL in editor
- Display the reference missing notification mark on the inspector in editor 
- Multi click to select the belowing nodes function on the scene panel in editor
- Texture atlas on the specified directory
- Imporve the server's extendable function in editor
- Remove the invalid project from the recent list automactically

### News
- Add 4 methods(playForward, playGroupForward, playReverse and playGroupReverse) for Tween class
- Add fading out effect for game loading UI
- Add customizable loading text for game loading UI
- Add 'Play from Entry' menu function in editor
- Add the selectable and editable function in editor when playing game
- Add the function to drag the prefab from project into the scene and hierarchy to create node

### Bug Fixes
- Fix the Unix-like system's bug in editor, see [Unable to create project with Ubuntu](https://github.com/qiciengine/qiciengine/issues/1) 
- Fix the CacheAsBitmap's wrong display issue on some mobile browsers
- Fix the wrong clip of the UIText's left-top outline and shadow 
- Fix the UIText's duplicated draw shadow issue
- Fix the bug that div element still exists when the Dom node is destoryed 
- Fix the context menu's wrong selection state on the windows Chrome browser in editor
- Fix the context menu's exception on the Safari browser
- Fix the exception when displaying the Prefab array type on the inspector in editor
- Fix the wrong JavaScript files dependency bug

## 2015-12-21, Version 1.0.3

### Downloads
[QICI Engine v1.0.3](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.3.zip)

### Enhancements
- ToggleGroup component add allowSwitchOff property 
- Create node by dragging from the toolbar button to the scene or hierarchy panel
- Create image by dragging from the texture in the project to the scene or hierarchy panel 
- Add locking node function in editor
- Improve Advert plugin
- Improve opening project panel and support adding specific folder as favority
- Limit deleting and renaming the project folder name in the project panel
- Improve the TableView plugin by adding pivot support
- Refactory the JavaScript files dependency

### News
- Add WebSocket server plugin
- Integrate API docs with Inspector panel for displaying tooltips
- Add remote log function for debugging
- Add application cache support for publishing
- Add search filtering function for hierarchy panel

### Bug Fixes
- Fix the NodeMask error when the height or width is 0
- Fix the wrong displaying anchor triangles when the parent's height or width is 0
- Fix the error when after editing script when previewing prefab
- Fix editing frame animation problem when the texture atlas is deleted
- Fix the circular dependencies issue caused when mutual reference in prefabs

## 2015-12-11, Version 1.0.2

### Downloads
[QICI Engine v1.0.2](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.2.zip)

### Enhancements
- Display User friendly error messages during exception in editor
- Find a workaround to avoid a iframe size bug on iOS 

### News
- Add WeChat share function in server plugin
- Add frame rate setting function in project settings

### Bug Fixes
- Fix the timer event lost bug
- Fix the loading assets fail bug when uncheck runInBackground in editor
- Fix the stack overflow bug in AspectRatioFitter component

## 2015-12-7, Version 1.0.1

### Downloads
[QICI Engine v1.0.1](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.1.zip)

### News
- Added a [Baidu AD Union](http://union.baidu.com/) plugin

### Bug Fixes
- Fix a bug that could cause game to be stuck in loading screen
- Fix the wrong saving scene when previewing game 
- Fix the empty entry scene name when publishing
- Fix a bug in the Lock Orientation plugin 

## 2015-12-4, Version 1.0.0

### Downloads
[QICI Engine v1.0.0](https://github.com/qiciengine/qiciengine/raw/master/releases/qiciengine-1.0.0.zip)

The first official release! Many thanks to all those who participated in, a special thank you to our core team members. 


