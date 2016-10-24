# storyboard-designable
A helpful set of extensions and subclasses for easier Storyboard UI design on both macOS and iOS projects

## Extension on `UIView`/`NSView`

We provide an extension on both `UIView` and `NSView` which adds the following properties as IBDesignables in Interface Builder:

- Border Color (`UIColor`/`NSColor`)
- Border Width (`CGFloat`)
- Corner Radius (`CGFloat`)
- Shadow:
  - Color (`UIColor`/`NSColor`)
  - Opacity (`CGFloat`)
  - Offset (`CGPoint`)
  - Radius (`CGFloat`)
  
Please note, all though these will be available in Interface Builder, they will not render in a storyboard unless you change your view's class to be of class `TSCView`, when you will get to see exactly how your layout looks directly in Interface Builder.

## Buttons

We provide a standard button style, which can be used by using the custom class `TSCButton` (And `TSCPopupButton` on macOS), which adds the following properties:

- Use Border Color (`Bool`): Forces the button to use the border color from the `UIView`/`NSView` extension
- Primary Color (`UIColor`/`NSColor`)
- Secondary Color (`UIColor`/`NSColor`)
- Solid Mode (`Bool`) Whether the button should be solid, or bordered
- Edge Insets (`CGSize`) Adds extra edge insets to the button

We provide two types of buttons: Solid and Bordered
### Solid Buttons
Use Primary Color as the background color, and secondary color as the title color.

### Bordered Buttons
Use Primary Color as the border color, and secondary color as the title color.

## UITextField

Adds the property `textInsets` for adding custom insets to the text field.

