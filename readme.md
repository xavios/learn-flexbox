## Flexbox learning

https://css-tricks.com/snippets/css/a-guide-to-flexbox/
https://flexboxfroggy.com/

### Properites that can be set on the flex container

`flex-direction` --> defines the main axis and cross axis.

`flex-dirction: row` is the default. In this case the main axis is from left to right.
The cross axis in this case is top to bottom.

`column` --> main axis is top to bottom, cross axis is left to right.
`row-reverse` --> main axis is right to left
`column reverse` --> main axis is bottom to top.

`flex-wrap` is a property of the flex container. By default there is `nowrap`.
When setting it to `wrap`, then still the flex items stretch across the corss axis.
`wrap-reverse` also exists.

`justify-content` --> how the items are aligned on the main axis. `flex-start` is the default.
We have `flex-end`, `space-between`, `space-around`, `space-evenly`.

`align-items` aligns the items on the cross axis. Default is `stretch`. We have `center`,
`flex-start`, `flex-end`, `baseline`. `baseline` makes sure that the items are pushed together
on the same base line on the corss axis.

`align-content` only takes effect once the `flex-wrap` is set to `wrap` or `wrap-reverse`.
This property takes effect on the extra space on the cross axis.

### Properites that can be set on the flex item

`order` is a property on the flex item. You can use it to move a DOM element with CSS, without
moving it in the actual DOM. Default is `order: 0`. Also works with negative numbers as well.

With `align-self` for an individual item you can overwrite the `align-items` property.
