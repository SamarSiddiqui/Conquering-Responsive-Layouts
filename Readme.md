## 21-Day Challenge of Building a Responsive Mindset

## Websites are inherently responsive; it's the styling that can make them unresponsive.



- Always use percentage width for block-level elements (BLEs), which default to 100% width.
- It's advisable to refrain from setting heights, as they can cause issues, with elements inside potentially overflowing as the viewport size decreases. Instead, maintain height by applying padding to elements.


### em vs rem
- When applied to font size, em units compound relative to their parent's font size. When applied to padding or margin, em units are relative to the element's font size.
- Width issues can arise on larger screens, leading to elements becoming excessively large. To maintain a specific size, utilize max-width.
- The difference between veiw w/h and percent width/height is that vw/h is relative to the viewport and % w/h is relative to parent dimensions. 


### FlexBox

- Applying display:flex creates a flex container with the default behavior of a row (flex-direction: row).
- If a parent div contains three children, the parent div becomes the flex container, and the children become flex items.
- Flex items naturally strive to be as small as possible.
- To create space between flex items, utilize gap.
- Instead of assigning fixed heights to elements, maintain gaps between them by using padding on the top and bottom.
- When using images in a flex container, enclose them in a div and set the div's width as needed (in percentage), while avoiding setting the height. Then, set the width of the image (also in percentage).
- Ensure image responsiveness by selecting an image and setting max-width: 100%. This ensures images never exceed their original size but shrink proportionally if the parent container shrinks.


 #### Properties of Flex Container:
 - **flex-wrap** by default is set to nowrap, **justify-content** by default is set to flex-start, and it always focuses on the Main Axis. **align-items** by default is set to stretch and always focuses on the Cross Axis.
- **flex-flow** is a shorthand property for flex-direction and flex-wrap.

#### Properties of Flex-items:
- **flex-grow** default is 0. It specifies how much the item will grow relative to the rest of the flexible items inside the same container.
- **flex-shrink** default is 1, specifies how the item will shrink relative to the rest of the flexible items inside the same container.
- **flex-basis**: 200px; describes how much space it will take, and shorthand for all three is flex: grow shrink basis; align-self aligning the items itself only.










