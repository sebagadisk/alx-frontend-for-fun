# Sass & Scss
## Learning Objectives
* What Sass means
* How to write Sass & Scss file
* What is the difference between Sass and Scss
* What is the Sass preprocessing
* How to declare a variable
* How to use nested definition
* How to import a Sass file
* How to use mixins
* How to declare extend/inheritance styles
* How to manipulate operators

### [0. Always debugging](./0-debug_log.scss)
Write a Sass file that prints Hello world in the debug output.
```
guillaume@ubuntu:~/$ sass 0-debug_log.scss | head -n 0
0-debug_log.scss:2 DEBUG: Hello world
guillaume@ubuntu:~/$

```

### [1. Color variable](1-color_variable.scss)
Write a Sass file that assigns the text color #3D3D3D to the HTML tags body and p.
- You must use a Sass variable

```
guillaume@ubuntu:~/$ sass 1-color_variable.scss | tail -n +2
body {
  color: #3D3D3D; }

p {
  color: #3D3D3D; }
guillaume@ubuntu:~/$
```

### [2. Colors](2-color_variables.scss)
Write a Sass file that assigns:
- The text color #3D3D3D to the HTML tags body and p
- The background color #6D6D6D to the HTML tags body and h2
- You must use 2 Sass variables
```
guillaume@ubuntu:~/$ sass 2-color_variables.scss | tail -n +2
body {
  color: #3D3D3D;
  background-color: #6D6D6D; }

p {
  color: #3D3D3D; }

h2 {
  background-color: #6D6D6D; }
guillaume@ubuntu:~/$
```

### [3. Nested tag](3-nested_tag.scss)
Write a Sass file that assigns:

- No margin or padding in body tags
- Margin 10px to all of the p tags inside body tags
- You must use nested declarations
```
guillaume@ubuntu:~/$ sass 3-nested_tag.scss | tail -n +2
body {
  margin: 0px;
  padding: 0px; }
  body p {
    margin: 10px; }
guillaume@ubuntu:~/$
```

### [4. Nested class](./4-nested_class.scss)
Write a Sass file that assigns:

- Text color #3D3D3D to elements inside body tags
- Text color #FF0000 to any elements of class .red inside body tags
- You must use nested declarations
```
guillaume@ubuntu:~/$ sass 4-nested_class.scss | tail -n +2
body {
  color: #3D3D3D; }
  body .red {
    color: #FF0000; }
guillaume@ubuntu:~/$
```

### [5. Nested child ](./5-nested_child.scss)
Write a Sass file that assigns:

- Text color #3D3D3D to elements inside body tags
- Text color #FF0000 to any elements of class .red that are the first children of the body
- You must use nested declarations

### [6. Nested hover](./6-nested_hover.scss)
Write a Sass file that assigns:

- Text color #FF0000 to button tags
- When the user hovers over button tags, text color should change to #00FF00
- You must use nested declarations

### [7. Nested and nested again](./7-nested_deeper.scss)
Write a Sass file that assigns:

- Font size 14px to all body tags
- Font size 16px to all h1 tags inside body tags
- Font size 12px to h1 tags of class .smaller inside body tags
- You must use nested declarations

### [8. Margin mixin ](8-mixin_margins.scss)
Write a Sass file that assigns:

- Margin left and right at 10px to body tags
- Margin left and right at 15px to div tags
- You must use a mixin

### [9. Extended](./9-extend_list.scss)
Write a Sass file that assigns:

- Font size 12px to all tags of class .info
- Text color #00FF00 to all tags of class .success and extend style of the class .info
- Text color #FF0000 to all tags of class .warning and extend style of the class .info

### [10. Import colors](./10-import_colors.scss)
Write a Sass file that assigns:

- Text color $red from 10-colors.scss to the class .red
- Text color $green from 10-colors.scss to the class .green
- Text color $blue from 10-colors.scss to the class .blue
- You must use @import

### [11. For Each](./11-loop_photos.scss)
Write a Sass file that creates a class for each name in the list $list-names and assigns the background image based on the name (example below):

- You must use @import
- You must use @each statement

### [12. Loop Headers](./12-loop_header.scss)
Write a Sass file that creates H* tags, where ‘*’ is the size of the font used.

- h1 must have font size equal to 1px, h2 must have font size equal to 2px, etc.
- You must create H* tags from 1 to 5
- You must use @for statement

### [13. Columns and operators](./100-loop_col.scss)
Write a Sass file that creates classes with different width:

- col-1 with width equals to 100%
- col-2 with width equals to 50%
- col-3 with width equals to 33.3333333333%
- col-4 with width equals to 25%
- You must create .col-* class from 1 to 4
- You must use a @for statement

### [ 14. Media query #0 ](./101-media_query.scss)
Write a Sass file that assigns:

- Font size 20px to h1 tags
- Font size 14px to h1 tags, when your screen width is smaller than 320px

---

## Author
* **Sebagadis Kahsay** - [sebagadisk](https://github.com/sebagadisk)
