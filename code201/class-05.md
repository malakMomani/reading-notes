# Chapter 5 : IMAGES

**you might want to include a picture inside your web page such as ; logo, photograph,illustration, diagram, or chart**

- Adding Images :
> < img src ="img/ASAC.jpg" alt ="ASAC" title="What is ASAC for example" />

- It takes 3 attributes:
  1. **src** : where your image is .
  2. **alt** : text description of the image which describes the image if you cannot see it .
  3. **title** :  provide additional information about the image , p when the user hovers over the image.

- Where to place images in your code :
  1. before a paragraph.
  2. inside the start of a paragraph.
  3. in the middle of a paragraph.

- Rules for creating images :
  1. Save images in the right format
  2. Save images at the right size
  3. Use the correct resolution.

- Correct format :
  1. **JPEG** : should use it when you have many different colors in a picture
  2. **GIF or PNG** : should when saving images with few colors or large areas of the same color.

- **Image Dimensions**
> The images you use on your website should be saved at the same width and height that you want them to appear on the page. 

- **Cropping Images**
> When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

- **Image Resolution**
> Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.
 
- **Vector Images**
> Vector images differ from bitmap images and are resolution-independent.

- **Animated GIFs**
> Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.

- **Transparency**
> Creating an image that is partially transparent (or "see-through") for the web.

# Chapter 11 : COLOR

**Every color on a computer screen is created by ixing amounts of red, green, and blue. To find the color you want, you can use a color picker.**

![rgb](/mnt/c/Users/ALI/Desktop/reading-notes/pics/rgb_palette.png)

- **rgb values** : `example: rgb(3,66,90)`
- **hex codes** : ` For example: #ee3e80`
- **color names** : `example : lightblue`
- **Hue** : Hue is near to the colloquial idea of color.
- **Saturation** : The amount of the color you want.
- **Brighteness** : How much color is in . 
- opacity, rgba : ` rgba(50,2,100,0.5);` value between 0.0 and 1.0
- **hsl,hsla**: hue , saturation , lighteness
`hsl(0,0%,78%)`
`hsla(0,100%,100%,0.5)`

# Chapter 12 : TEXT

- **Typeface Terminology**
  - Serif . ![serif](pics/serif.png)
  - Sans-Serif . ![sans-serif](pics/sans_serif.png)
  - Monospace. ![monospace](pics/mono.png)

**WEIGHT** | **STYLE** | **STRETCH**
------------ | ------------- | ------------
Light | Normal | Condensed
Medium | Italic | Regular
Bold | Oblique | Extended
Black | | 

- **font-family** : specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

- **font-size** : `font-size: 12px;`
- **@font-face**
```
@font-face {
font-family: 'ChunkFiveRegular';
src: url('fonts/chunkfive.eot');}
```
- **font-weight** : *normal* or *bold* .
- **font-style** : *normal* or *italic* or *oblique*.
- **text-transform** : *uppercase* or *lowercase* or *capitalize*
- **text-decoration** : *none* or *underline* or *overline* or *line-through* or *blink*

# [CODE201](https://malakmomani.github.io/reading-notes/code201/home)
