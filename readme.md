# React Native Styling Cheat Sheet

React Native styling material in one page. Imported from the [react-native style props](https://facebook.github.io/react-native/docs/layout-props).

### Table of Contents

- [Flex](https://github.com/anujjangid/react-native-styling-cheat-sheet/#flex-properties)
- [Margin](https://github.com/anujjangid/react-native-styling-cheat-sheet/#margin-properties)
- [Padding](https://github.com/anujjangid/react-native-styling-cheat-sheet/#padding-properties)
- [Border](https://github.com/anujjangid/react-native-styling-cheat-sheet/#border-properties)
- [Border Radius](https://github.com/anujjangid/react-native-styling-cheat-sheet/#border-radius-properties)
- [Mixed](https://github.com/anujjangid/react-native-styling-cheat-sheet/#mixed-properties)
- [Flex 0 & Flex 1](https://github.com/anujjangid/react-native-styling-cheat-sheet/#react-native-style-properties-with-flex0-and-flex1)
- [Stylesheet Creation](https://github.com/anujjangid/react-native-styling-cheat-sheet/#basic-stylesheet-creation)
- [Stylesheet Usage](https://github.com/anujjangid/react-native-styling-cheat-sheet/#how-to-use-the-stylesheet)
- [Device Utilities](https://github.com/anujjangid/react-native-styling-cheat-sheet/#device-utilities)

## Flex Properties

| **Name**       |                                         **Type**                                          | **Default Value** | **Description**                                                                                                                                                                                                                                                                                            |
| :------------- | :---------------------------------------------------------------------------------------: | :---------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Flex           |                                          Number                                           |         0         | React Native flex is entirely different if you compare with `css-flex`                                                                                                                                                                                                                                     |
| flexDirection  |                Any one of `row`, `row-reverse`, `column`, `column-reverse`                |     `column`      | `flexDirection` controls the direction of childrens, `row` works from left to right, column works from top to bottom                                                                                                                                                                                       |
| flexBasis      |                                          number                                           |         0         | --                                                                                                                                                                                                                                                                                                         |
| flexGrow       |                                          number                                           |         0         | --                                                                                                                                                                                                                                                                                                         |
| flexShrink     |                                          number                                           |         0         | --                                                                                                                                                                                                                                                                                                         |
| flexWrap       |                               Any one of `wrap` , `nowrap`                                |     `nowrap`      | Controls if children can wrap itself when they reach to the end of the flex conatiner                                                                                                                                                                                                                      |
| justifyContent |      Any one of `flex-start`, `flex-end`, `center`, `space-between`, `space-around`       |   `flex-start`    | Depends on the parent flex direction, can adjust children vertically or horizontally                                                                                                                                                                                                                       |
| alignItems     |           Any one of `flex-start`, `flex-end`, `center`, `stretch`, `baseline`            |     `stretch`     | `alignItems` aligns children in the cross direction. For example, if children are flowing vertically, `alignItems` controls how they align horizontally. It works like `align-items` in CSS (default: stretch). See [Here](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items) for more details. |
| alignContent   | Any one of `flex-start`, `flex-end`, `center`, `stretch`, `space-between`, `space-around` |        --         | `alignContent` controls how rows align in the cross direction, overriding the alignContent of the parent. See [Here](https://developer.mozilla.org/en-US/docs/Web/CSS/align-content) for more details.                                                                                                     |
| alignSelf      |       Any one of `auto`, `flex-start`, `flex-end`, `center`, `stretch`, `baseline`        |      `auto`       | `alignSelf` controls how a child aligns in the cross direction, overriding the alignItems of the parent. It works like align-self in CSS. See [Here](https://css-tricks.com/almanac/properties/a/align-self/) for more details.                                                                            |
| direction      |                            Any one of `inherit`, `ltr`, `rtl`                             |     `inherit`     | `direction` direction specifies the directional flow of the user interface. The default is inherit, except for root node which will have value based on the current locale. See [Here](https://facebook.github.io/yoga/docs/rtl/) for more details.                                                        |

## Margin Properties

| **Name**         | **Type** | **Default Value** | **Description**                                                                                                                                                                     |
| :--------------- | :------: | :---------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| margin           |  number  |         0         | Set `margin` on each corner (top,right,bottom,left)                                                                                                                                 |
| marginTop        |  number  |         0         | Works same as in css `margin-top`                                                                                                                                                   |
| marginRight      |  number  |         0         | Works same as in css `margin-right`                                                                                                                                                 |
| marginBottom     |  number  |         0         | Works same as in css `margin-bottom`                                                                                                                                                |
| marginLeft       |  number  |         0         | Works same as in css `margin-left`                                                                                                                                                  |
| marginHorizontal |  number  |         0         | Set `margin` on left and right                                                                                                                                                      |
| marginVertical   |  number  |         0         | Set `margin` on top and bottom                                                                                                                                                      |
| marginStart      |  number  |         0         | Works on the basis of the direction, If the direction is `ltr`, `marginStart` is equivalent to `marginLeft`. When direction is `rtl`, `marginStart` is equivalent to `marginRight`. |
| marginEnd        |  number  |         0         | Works on the basis of the direction, If the direction is `ltr`, `marginEnd` is equivalent to `marginRight`. When direction is `rtl`, `marginEnd` is equivalent to `marginLeft`.     |

## Padding Properties

| **Name**          | **Type** | **Default Value** | **Description**                                                                                                                                                                         |
| :---------------- | :------: | :---------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| padding           |  number  |         0         | Set `padding` on each corner (top,right,bottom,left)                                                                                                                                    |
| paddingTop        |  number  |         0         | Works same as in css `padding-top`                                                                                                                                                      |
| paddingRight      |  number  |         0         | Works same as in css `padding-right`                                                                                                                                                    |
| paddingBottom     |  number  |         0         | Works same as in css `padding-bottom`                                                                                                                                                   |
| paddingLeft       |  number  |         0         | Works same as in css `padding-left`                                                                                                                                                     |
| paddingHorizontal |  number  |         0         | Set `padding` on left and right                                                                                                                                                         |
| paddingVertical   |  number  |         0         | Set `padding` on top and bottom                                                                                                                                                         |
| paddingStart      |  number  |         0         | Works on the basis of the direction, If the direction is `ltr`, `paddingStart` is equivalent to `paddingLeft`. When direction is `rtl`, `paddingStart` is equivalent to `paddingRight`. |
| paddingEnd        |  number  |         0         | Works on the basis of the direction, If the direction is `ltr`, `paddingEnd` is equivalent to `paddingRight`. When direction is `rtl`, `paddingEnd` is equivalent to `paddingLeft`.     |

## Border Properties

| **Name**          | **Type** | **Default Value** | **Description**                                                                                                                                                                                     |
| :---------------- | :------: | :---------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| borderTopWidth    |  number  |         0         | Works same as in css `border-top-width`                                                                                                                                                             |
| borderRightWidth  |  number  |         0         | Works same as in css `border-right-width`                                                                                                                                                           |
| borderBottomWidth |  number  |         0         | Works same as in css `border-bottom-width`                                                                                                                                                          |
| borderLeftWidth   |  number  |         0         | Works same as in css `border-left-width`                                                                                                                                                            |
| borderEndWidth    |  number  |         0         | Works on the basis of the direction, If the direction is ltr, `borderEndWidth` is equivalent to `borderRightWidth`. When direction is rtl, `borderEndWidth` is equivalent to `borderLeftWidth`.     |
| borderStartWidth  |  number  |         0         | Works on the basis of the direction, If the direction is ltr, `borderStartWidth` is equivalent to `borderLeftWidth`. When direction is rtl, `borderStartWidth` is equivalent to `borderRightWidth`. |
| borderWidth       |  number  |         0         | Works same as in css `border-width`                                                                                                                                                                 |

## Border Radius Properties

| **Name**                | **Type** | **Required** | **Description** |
| :---------------------- | :------: | :----------: | :-------------: |
| borderTopLeftRadius     |  number  |    false     |       --        |
| borderTopRightRadius    |  number  |    false     |       --        |
| borderBottomLeftRadius  |  number  |    false     |       --        |
| borderBottomRightRadius |  number  |    false     |       --        |

## Mixed Properties

| **Name**  |             **Type**              |  **Default Value**   | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| :-------- | :-------------------------------: | :------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| width     |              number               |        auto\*        | `width` sets the width of this component. It works similarly to `width` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [http://www.w3schools.com/cssref/pr_dim_width.asp](http://www.w3schools.com/cssref/pr_dim_width.asp) for more details.                                                                                                                                                                                                                                                                                                                                       |
| height    |              number               |        auto\*        | `height` sets the height of this component. It works similarly to `height` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [http://www.w3schools.com/cssref/pr_dim_width.asp](http://www.w3schools.com/cssref/pr_dim_width.asp) for more details.                                                                                                                                                                                                                                                                                                                                    |
| maxWidth  |              number               |        auto\*        | `maxWidth` is the maximum width for this component, in logical pixels. It works similarly to `max-width` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [http://www.w3schools.com/cssref/pr_dim_max-width.asp](http://www.w3schools.com/cssref/pr_dim_max-width.asp)for more details.                                                                                                                                                                                                                                                                                               |
| maxHeight |              number               |        auto\*        | `maxHeight` is the maximum height for this component, in logical pixels. It works similarly to `max-height` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [http://www.w3schools.com/cssref/pr_dim_max-height.asp](http://www.w3schools.com/cssref/pr_dim_max-height.asp)for more details.                                                                                                                                                                                                                                                                                          |
| minWidth  |              number               |        auto\*        | `minWidth` is the minimum width for this component, in logical pixels. It works similarly to `min-width` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [http://www.w3schools.com/cssref/pr_dim_min-width.asp](http://www.w3schools.com/cssref/pr_dim_min-width.asp)for more details.                                                                                                                                                                                                                                                                                               |
| minHeight |              number               |        auto\*        | `minHeight` is the minimum height for this component, in logical pixels. It works similarly to `min-height` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [http://www.w3schools.com/cssref/pr_dim_min-height.asp](http://www.w3schools.com/cssref/pr_dim_min-height.asp)for more details.                                                                                                                                                                                                                                                                                          |
| top       |              number               |        auto\*        | `top` is the number of logical pixels to offset the top edge of this component. It works similarly to `top` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [https://developer.mozilla.org/en-US/docs/Web/CSS/top](https://developer.mozilla.org/en-US/docs/Web/CSS/top) for more details of how `top` affects layout.                                                                                                                                                                                                                                                               |
| right     |              number               |        auto\*        | `right` is the number of logical pixels to offset the right edge of this component. It works similarly to `right` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [https://developer.mozilla.org/en-US/docs/Web/CSS/right](https://developer.mozilla.org/en-US/docs/Web/CSS/right)for more details of how `right` affects layout.                                                                                                                                                                                                                                                    |
| bottom    |              number               |        auto\*        | `bottom` is the number of logical pixels to offset the bottom edge of this component. It works similarly to `bottom` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [https://developer.mozilla.org/en-US/docs/Web/CSS/bottom](https://developer.mozilla.org/en-US/docs/Web/CSS/bottom) for more details of how `top` affects layout.                                                                                                                                                                                                                                                |
| left      |              number               |        auto\*        | `left` is the number of logical pixels to offset the left edge of this component. It works similarly to `left` in CSS, but in React Native you must use logical pixel units, rather than percents, ems, or any of that. See [https://developer.mozilla.org/en-US/docs/Web/CSS/left](https://developer.mozilla.org/en-US/docs/Web/CSS/left) for more details of how `left` affects layout.                                                                                                                                                                                                                                                         |
| zIndex    |              number               | auto\*(Not required) | `zIndex` controls which components display on top of others. Normally, you don't use `zIndex`. Components render according to their order in the document tree, so later components draw over earlier ones. `zIndex` may be useful if you have animations or custom modal interfaces where you don't want this behavior. It works like the CSS `z-index` property - components with a larger `zIndex` will render on top. Think of the z-direction like it's pointing from the phone into your eyeball. See [https://developer.mozilla.org/en-US/docs/Web/CSS/z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index) for more detail. |
| display   |     Any one of `flex`, `none`     |        `flex`        | display sets the display type of this component.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| position  | Any one of `relative`, `absolute` |      `relative`      | `position` in React Native is similar to regular CSS, but everything is set to `relative` by default, so `absolute` positioning is always just relative to the parent.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

## React Native style properties with flex:0 and flex:1

## **Flex: 0**

- **flex: 0**
  - Element takes the size of contents. According to the [documentation](https://facebook.github.io/react-native/docs/layout-props.html#flexgrow) it should be sized by setting width and height props but it seems to fit to contents if those aren't set.
- **flex: 0, flexBasis: {{px}}**
  - Element takes the size given by flexBasis
- **flex: 0, flexGrow: 1**
  - with flex: 0 and flexGrow: 1; it's the same as adding the size of the contents (in the example above it's a ) to the size of an element that's set to flex: 1. It's similar to flex: 1, flexBasis: 10 except instead of adding a number of pixels you're adding the size of the content.
- **flex: 0, flexShrink: 1**
  - With flex: 0 and flexShrink: 1, the element seems to take the size of the content, in other words it's the same as just flex: 0. I'll bet there are situations where it would be bigger than the content but I haven't see that yet.
- **flex: 0, flexGrow: 1, flexBasis: {{px}}**
  - This is the same as flex: 0, flexGrow: 1 except instead of adding the content size to a flex: 1 element it adds the given number of pixels.
- **flex: 0, flexShrink: 1, flexBasis: {{px}}**
  - This is the same as flex: 0, flexBasis: {{px}}.
- **flex: 0, height: {{px}}**
  - With flex: 0, height is treated just like flexBasis. If there is both a height and flexBasis are set, height is ignored.

#### **Flex: 1**

- **flex: 1**
  - Element takes available space. See [documentation](https://facebook.github.io/react-native/docs/layout-props.html#flexgrow) for more details
- **flex: 1, flexBasis: {{px}}**
  - With flex: 1 and flexBasis: {{px}}; the value of flexBasis is added to the element's size. In other words, it's like taking a flex: 1 element and adding on the number of pixels set by flexBasis. So if a flex: 1 element is 50px, and you add flexBasis: 20 the element will now be 70px.
- **flex: 1, flexGrow: 1**
  - ignored
- **flex: 1, flexShrink: 1**
  - ignored
- **flex: 1, flexGrow: 1, flexBasis: {{px}}**
  - This is the same as flex: 1, flexBasis: {{px}} since flexGrow is ignored.
- **flex: 1, flexShrink: 1, flexBasis: {{px}}**
  - This is the same as flex: 1, flexBasis: {{px}} since flexShrink is ignored.
- **flex: 1, height: {{px}}**
  - With flex: 1, height is ignored. Use flexBasis instead.

## Basic stylesheet creation

```javascript
export const newStyle = {
    fontWeight: "bold",
}
// import { StyleSheet } from 'react-native'
// To create style in react-native, we need to import Stylesheet, as mentioned above
var styles = StyleSheet.create({
  block: {
    width:420,
    height:200
  },
  text: {
      color:'#4286f4'
  }
  // Extend style from exported style
  button:{
      ...newStyle,
      width:200,
  }
});
```

## How to use the stylesheet

```javascript
// Stylesheet from the styles object
<View style={styles.block}>
  <Text style={styles.text}>Style from styles object</Text>
</View>
// Inline style
<View style={width:100, height:100}>
   <Text style={color:'#4286f4'}>Inline style</Text>
</View>
//  # Extending and overriding styles with inline styles
<View style={[styles.block, { width: 500 }]}>
  <Text style={styles.text}>Style Combine with style object and inline</Text>
</View>
```

## Device Utilities

```javascript
import { Dimensions, Platform, PixelRatio } from 'react-native';

export const DeviceSizes = {
  SMALL: 0,
  MEDIUM: 1,
  LARGE: 2,
};

export function isIphoneX() {
  const dimen = Dimensions.get('window');
  return (
    Platform.OS === 'ios' &&
    (dimen.height === 812 || dimen.height === 896) &&
    dimen.width === 375
  );
}

const pixelRatio = PixelRatio.get();

const { height, width } = Dimensions.get('window');

const size = () => {
  switch (width) {
    case 320:
      return DeviceSizes.SMALL;
    case 375:
      return DeviceSizes.MEDIUM;
    case 414:
      return DeviceSizes.LARGE;
    default:
      return DeviceSizes.MEDIUM;
  }
};

export default {
  size: size(),
  height,
  width,
  isIphoneX: isIphoneX(),
  pixelRatio,
};
```
