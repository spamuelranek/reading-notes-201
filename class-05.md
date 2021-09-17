# Pics or it doesn't Look Good, That *COLOR* looks good on you, **TEXT** you later

## Pictures
### Choosing the Right Type of Picture
- Often there is a struggle to pick the right picture
  - But what if I told you there is an important question to ask even after you found the perfect picture
  - *what format is the picture?*
    - If you are using a real life picture : recommend using JPEG - lossy compression
      - can represent 16 million colors
      - loss comes from taking an average value of color
    - logos and line art : recommend using PNG - lossless compression
      - PNG8 can do 256 colors
      - PNG24 can do 16 million
      - works well with transparency
    - animation pieces : recommend using GIF - lossless compression
      - can represent 256 colors
      - has lower resolution
- `<img src="Picture of cute flowers.jpg" alt="Three Yellow Flowers">`
  - `<img>` is the image tag
  - `src=` is an attribute for source
  - `"Picture of cute flowers.jpg"` is the picture that is being sourced. This can be a path or a url
  - `alt = "Three Yellow Flowers"` is a short description if you can not see the picture

## CoL**o**_r_
### Understanding COLOR
- all color on your screen is a combination of Red, Blue, or Green (RGB)
- Color along with pictures are one of the many visiual tools designers use to share information without writing anything
  - it can be crucial to helping set a tone or feeling the webpage
- Color Values
  - RGB
    - individual amount of Red, Green, and Blue in a scale of 0-255
    - `(125,210,25)`
  - Hex Codes
    - same individual amount of Red, Green, and Blue in a scale of 0-255 but expressed in hexdecimal code
    - `#66cdaa`
  - Color Names
    - 147 color names are supported by browsers
- Extra vocab: Hue, Saturations-gray"scale", darkness-black"scale"

# Texts from last night
- Typeface terminology
  - serif
    - tiny flags
  - sans-serif
    - no tiny flags
    - often thought to be more modern design
  - monospace
    - every letter has the same widths
- each typeface may have a different default that a browser uses.
  - you can set precedence with
    - `font-family: Georgia, Times, serif;`
    - serif being the generic font
- pt=px or close enough
  - most browsers default to 16 pixels which would be 1 em
  - Ledding-space between lines of text
  - Kerning-space between each letter
- Additional Attribute Selectors
  - `[]` can target any specific attribute of a html tag
  - `[=]` can target any specific attribute = a specific value


