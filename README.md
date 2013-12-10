# JSFlatButton

A simple, light-weight, flat design UI button for iOS.

![FlatButton Screenshot 1][img1] &nbsp;&nbsp;&nbsp;&nbsp; ![FlatButton Screenshot 2][img2]

## About

Following recent design trends toward flat design. Get hip. Embrace minimalism.

* Simple, easy-to-use sublcass of `UIButton`
* iOS 5.0+, ARC, Universal, Retina, Storyboards
* Make flat buttons with text and/or images

### Icons
Free icons designed by [Darran Morris](https://twitter.com/darranmorris) at [APP-BITS](http://app-bits.com). **Go show him some [love](http://store.app-bits.com).**

**READ: [App-Bits License][link1] and [App-Bits README][link2] for details on icon usage.**

## Installation

Drag the `JSFlatButton/` folder to your project

## How To Use

* Initialize buttons
	* To create buttons programmatically:
		* Call `initWithFrame: backgroundColor: foregroundColor:`
		* Or, use the [UIButton][ref1] methods `buttonWithType:` with `UIButtonTypeCustom`, or `initWithFrame:`
	* To create buttons with Storyboards:
		* Drag a `UIButton` to your view
		* Set its class to `JSFlatButton` and button type to `Custom` in Interface Builder
		* Set your `IBOutlet` and `IBAction` accordingly
* Set button properties `buttonBackgroundColor` and `buttonForegroundColor`
* **Colors must be set in HSB or RGB color space**
	* Use the [UIColor][ref2] methods: `colorWithHue: saturation: brightness: alpha:` or `colorWithRed: green: blue: alpha:`
	* iOS built-in colors **will not** work (e.g., `[UIColor whiteColor]`, `[UIColor darkGrayColor]`, etc.)
* Call `setFlatTitle:` and `setFlatImage:` to set the button title and image, respectively
* You may set your button title font and other attributes as you normally would with `UIButton`
* *Special Options*
	* Set `shouldHighlightImage` to `YES` to optionally highlight the button image when pressed (default value is `NO`)
	* Set `shouldHighlightText` to `YES`to optionally highlight the button title text when pressed (default value is `NO`)
	* To make a flat button with an *image-only* and **no** background color:
		* Set `buttonBackgroundColor` to `nil`
		* Set `shouldHighlightImage` to `YES`
		* Set your `buttonForegroundColor` to whatever you want
		* Call `setFlatTitle:` with `nil`
	* Similarly, you can make a flat button with *text-only* and **no** background color
* See included demo project: `FlatButtonDemo.xcodeproj` 

## Apps Using This Control

[Eight-Twelve](https://itunes.apple.com/us/app/eight-twelve/id648715570?mt=8)

*[Contact me](mailto:jesse.squires.developer@gmail.com) to have your app listed here.*

## [MIT License](http://opensource.org/licenses/MIT)

You are free to use this as you please. No attribution necessary. **However, a link back to [Hexed Bits](http://www.hexedbits.com) or here would be appreciated. If you use this, please tell me about it!**

Copyright &copy; 2013 Jesse Squires

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### Icons

**READ: [App-Bits License][link1] and [App-Bits README][link2] for details on icon usage.**

[img1]:https://raw.github.com/jessesquires/FlatButton/master/Screenshots/screenshot-iphone4-1.png
[img2]:https://raw.github.com/jessesquires/FlatButton/master/Screenshots/screenshot-iphone4-2.png

[ref1]:http://developer.apple.com/library/ios/#DOCUMENTATION/UIKit/Reference/UIButton_Class/UIButton/UIButton.html
[ref2]:http://developer.apple.com/library/ios/#documentation/uikit/reference/UIColor_Class/Reference/Reference.html

[link1]:https://github.com/jessesquires/FlatButton/blob/master/App-Bits%20Icons/00_License.txt
[link2]:https://github.com/jessesquires/FlatButton/blob/master/App-Bits%20Icons/00_readme.pdf


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/jessesquires/flatbutton/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

