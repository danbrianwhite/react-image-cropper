## React Image Cropper

[![Downloads](https://img.shields.io/npm/dt/react-image-cropper.svg)](https://www.npmjs.com/package/react-image-cropper)
[![Version](https://img.shields.io/npm/v/react-image-cropper.svg)](https://www.npmjs.com/package/react-image-cropper)

A React.JS Image Cropper
Touch supported

**[See the demo](http://braavos.me/react-image-cropper/)**

Custom:

+ initial cropper frame position 
+ frame width, height, rate
+ crop event

### How to Use

+ `import {Cropper} from 'react-image-cropper'`

+ styles are all inline

+ define Cropper with src, and ref to execute crop method  

```
<Cropper src="http://braavos.me/images/posts/college-rock/the-smiths.png" ref="cropper"/>
```

+ crop and get image url

`image.src = this.refs.cropper.crop()`

+ get crop values

`var values = this.refs.cropper.values()`

+ custom use

| prop  |  value   |
|:-------:|:--------|
| rate | width / height |
| disabled | boolean |
| width | cropper frame width |
| height | cropper frame height |
| originX | cropper original position(x axis)|
| originY | cropper original position(Y axis)|
| selectionNaural | cropper frame sizes and position are relative to the image's natural size (bool default false) |
| fixedRatio | turn on/off fixed ratio (bool default true) |
| allowNewSelection | allow user to create a new selection instead of reusing initial selection (bool default true) |
| styles | specify styles to override inline styles |
| imageLoaded | specify fuction callback to run when the image completed loading |
| beforeImageLoaded | specify function callback to run when the image size value is ready but the image has not completed loading |
| imageLoadError | specify function callback to run when the image errors during loading |
| onDragStop | specify function callback to run when dragging the crop has ended |


**[See the demo](http://braavos.me/react-image-cropper/)**

