## 21 Days Challenge of Building Responsive Mindset
## Websites are already Responsive, by giving it style we make it UnResponsive.

- Always give width as percentage to block level element.(BLE have a defualt width of 100%)
- It's a good idea to avoid setting heights,as they cause more issue and elements inside them can peak outside as the vieport size decreases.(Maintain the height with giving Padding to the Element.)
### em vs rem
- em units when applied to fontsize on the element, it compound on each other as they look at their parents font size. And if we apply em to padding or margin than it looks (relative) to font size of the element itself.
- width can cause issue at larger screen as things cam get too big, so we can use max-width for maintaining a particular size.
- The difference between vw or vh and percent width and height is that vw/h is relative to the viewport and % w/h is relative to parent dimensions. 


### FlexBox

-  display:flex is going to make a flex container having default behaviour of row. (flex-direction:row).
-  If a Parent Div have three Children, then the parent div is the flex Container & Children Are the Flex Items.
- flex items by default want to be as small as they possibly can be.
- To create space between the flex-items we can use Gap.