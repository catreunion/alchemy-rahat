- develop a fully dynamic NFT with on-chain metadata that changes based on your interactions with it

- Polygon

  - built on top of Ethereum to solve some of the issues characterizing it - while relying on it to function

  - described as Layer 2 chains (L2)

  - a decentralized EVM compatible scaling platform

  - low transaction fees

  - PoS : lower gas fees and fast transactions

- SVG image

  - scalable vector graphic file

  - vector image : made up of points, lines, curves, and shapes based on mathematical formulas

  - written in XML : markup language specifing all of the shapes, colors, and text that comprise the image

  - convert a SVGs file into Base64 data for displaying in a web browser without the need for a hosting provider

  - Base64

    - **data:image/svg+xml;base64,**

      - data directives

      - tell the browser

        - the Base64 string is an SVG image

        - the browser will know how to handle the data

    - base64 data : the actuals data

- JSON object

  - the bytes type : a dynamically sized array of up to 32 bytes where you can store strings and integers

  - **abi.encodePacked()** transforms into an array of bytes

&nbsp;

```
////////////////////////////// a SVG file in plain text
<svg xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMinYMin meet" viewBox="0 0 350 350">
  <style>.base { fill: white; font-family: serif; font-size: 14px; }</style>
  <rect width="100%" height="100%" fill="black" />
  <text x="50%" y="40%" class="base" dominant-baseline="middle" text-anchor="middle">Warrior</text>
  <text x="50%" y="50%" class="base" dominant-baseline="middle" text-anchor="middle">Levels: getLevels(tokenId)</text>
</svg>

////////////////////////////// a SVG file converted into Base64 data
data:image/svg+xml;base64,IDxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiBwcmVzZXJ2ZUFzcGVjdFJhdGlvPSJ4TWluWU1pbiBtZWV0IiB2aWV3Qm94PSIwIDAgMzUwIDM1MCI+CiAgICAgICAgPHN0eWxlPi5iYXNlIHsgZmlsbDogd2hpdGU7IGZvbnQtZmFtaWx5OiBzZXJpZjsgZm9udC1zaXplOiAxNHB4OyB9PC9zdHlsZT4KICAgICAgICA8cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSJibGFjayIgLz4KICAgICAgICA8dGV4dCB4PSI1MCUiIHk9IjQwJSIgY2xhc3M9ImJhc2UiIGRvbWluYW50LWJhc2VsaW5lPSJtaWRkbGUiIHRleHQtYW5jaG9yPSJtaWRkbGUiPldhcnJpb3I8L3RleHQ+CiAgICAgICAgPHRleHQgeD0iNTAlIiB5PSI1MCUiIGNsYXNzPSJiYXNlIiBkb21pbmFudC1iYXNlbGluZT0ibWlkZGxlIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIj5MZXZlbHM6IGdldExldmVscyh0b2tlbklkKTwvdGV4dD4KICAgICAgICA8L3N2Zz4=
```
