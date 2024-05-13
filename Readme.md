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
- **margin:0,auto;** is a good way to make element center itself inside the container across Cross Axis.

#### min(),max(), clamp(), clac()

- **min(value1, value2, ...);**: This function returns the smallest value among the values provided. 

Ex: **width: min(200px, 50%);** This sets the width to the smallest value between 200 pixels and 50% of the parent element's width. So, it ensures that the width won't be smaller than 200 pixels.

- **max(value1, value2, ...);**: This function does the opposite of min(). It returns the largest value among the values provided. It's useful when you want to set a maximum limit. 

Ex: **font-size: max(16px, 2vw);**
This sets the font size to the largest value between 16 pixels and 2% of the viewport width. So, it ensures that the font size won't exceed 16 pixels even if 2% of the viewport width would result in a larger size.




- **clamp(min, actual, max)**: It's a smart way to set a value that stays within a certain range.

- min is the minimum value you want.
- actual is the value you want to use.
- max is the maximum value you want.

Ex: **font-size: clamp(16px, 4vw, 24px);**
This means the font size will be at least 16 pixels (min), but if the viewport width (actual) increases, it will grow, but won't go beyond 4% of the viewport width or 24 pixels, whichever is smaller (max).


- **calc(expression)** - We can use calc() to perform addition, subtraction, multiplication, and division within CSS property values.

Ex: **width: calc(50% - 20px);** This calculates the width to be 50% of its container minus 20 pixels. So, if the container is 1000 pixels wide, the width would be **480px** (50% of 1000 - 20).

**height: calc(100vh - 50px);**
This sets the height to be 100% of the viewport height minus 50 pixels.




