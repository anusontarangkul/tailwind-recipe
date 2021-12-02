# tailwind-recipe

An introducty app using tailwind for styling.

![screenshot](screenshot.png)

|                                         |                                         |                                                   |
| :-------------------------------------: | :-------------------------------------: | :-----------------------------------------------: |
|    [Introduction](#tailwind-recipe)     | [Table of Contents](#table-of-contents) | [Development Highlights](#development-highlights) |
|      [Installation](#installation)      |    [Page Directory](#page-directory)    |       [Code Hightlights](#code-highlights)        |
| [Technologies Used](#Technologies-Used) |           [Credits](#Credits)           |                [License](#License)                |

## Development Highlights

- Create custom reusable tailwind css
- Styling for different responsiveness
- Transitions
- Tailwind flex

## Installation

`npm i`

## Page Directory

There is a custom tailwind.config for custom styling. The files are built into public.

## Code Highlights

Create custom tailwind config

```JavaScript
module.exports = {
  purge: [],
  theme: {
    extend: {
      colors: {
        primary: '#FF6363',
        secondary: {
          100: '#E2E2D5',
          200: '#888883',
        }
      },
    },
    fontFamily: {
      body: ['Signika Negative']
    }
  },
  variants: {},
  plugins: [],
}
```

Create custom tailwind components

```CSS
@layer components {
  .card {
    @apply rounded bg-white border-gray-200 shadow-md overflow-hidden relative;
  }

  .badge {
    @apply absolute top-0 ml-2 p-2 mt-2 bg-secondary-100 text-secondary-200 text-xs uppercase font-bold rounded-full;
  }
  .btn {
    @apply rounded-full py-2 px-3 uppercase text-xs font-bold cursor-pointer tracking-wider;
  }
}
```

## Technologies

- [tailwind](https://tailwindcss.com/)

## Credits

The Tailwind [tutorial](https://www.youtube.com/watch?v=aQS7kaje-24&list=PL4cUxeGkcC9ht1OMQPhBVKAb2dVLhg-MJ) by The Net Ninja.

|                           |                                                                                                                                                                                                       |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **David Anusontarangkul** | [![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/in/anusontarangkul/) [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/anusontarangkul) |

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/)
