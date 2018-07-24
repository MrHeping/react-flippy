###React-Flippy


React-Flippy allows you to create flipping cards in React projects. 
It can be used as controlled or uncontrolled component.

![Vertical](hover_flippy.gif)

![Horizontal](toggle_flippy.gif)


[Live Demo](http://flippy.sbaydin.com "Live Demo")


####How to install ?

`npm install react-flippy` or `yarn add react-flippy`

####How to use ?

```javascript
import Flippy, { FrontSide, BackSide } from './../lib';
// ... component class
render() {
	// .. return
	<Flippy
		flipOnHover={false} // default false
		flipOnClick={true} // default false
		flipDirection="horizontal" // horizontal or vertical
		// and other props, which will go to div
		style={{ width: '200px', height: '200px' }}
  >
    <FrontSide
      style={{
        backgroundColor: '#41669d',
      }}
    >
      RICK
    </FrontSide>
    <BackSide
      style={{ backgroundColor: '#175852'}}>
      ROCKS
    </BackSide>
  </Flippy>
}
```

##API for Components

###Flippy
| Prop Name | Description   | Values  | Default   |
| :------------: | :------------: | :------------: | :------------: |
|  flipDirection | Direction of flip effect  |  horizontal/vertical | horizontal|
|  flipOnHover | Should card flip on mouse hover  |  true/false  |  false  |
|  flipOnClick   | Should card click on mouse click/touch  | true/false   | true  |
| ...props   | Other props will be passed to container.  |   |   |


###FrontSide

| Prop Name | Description   | Values  | Default   |
| :------------: | :------------: | :------------: | :------------: |
|  animationDuration | Duration of flip animation, should be used equal with back side for a good view.  |  number | 600 |
|  elementType | Dom element type for card  | dom element types  |  div  |
| ...props   | Other props will be passed to card.  |   |   |


###BackSide

| Prop Name | Description   | Values  | Default   |
| :------------: | :------------: | :------------: | :------------: |
|  animationDuration | Duration of flip animation, should be used equal with front side for a good view.  |  number | 600 |
|  elementType | Dom element type for card  | dom element types  |  div  |
| ...props   | Other props will be passed to card.  |   |   |


