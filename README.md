## Dev tools pages

This repository contains our dev tools pages.

## Local Dev Setup

Requires Node version 6.9.5 or higher & yarn v1.9.4

### 1. Install dependencies:

Make sure you install Yarn v1.9.4 (npm won't work!).

```bash
yarn install
```

### 2. Run dev server

```bash
yarn dev
```

Visit [http://localhost:3572/](http://localhost:3572/) in your browser.

The webpage will refresh when source code is changed.

### 3. Code!

There are some basic primitives we'd like you to use:

1.  `<Container>Stuff</Container>`: Use containers instead of divs,spans,etc... and use it's props instead of inline styles (e.g `style={{margin: 3}}` should be `margin="3px"`

2.  `<Text>Look ma, text!</Text>`: Use text components whenever rendering text. It has props for manipulating texts, so again no in-line styles. Use `fontColor="red"`, not `style={{color: 'red'}}`.

3.  Styled-components: See the `ui/button.tsx` file for an example of how to use these.

4.  BassCss: This library gives you access to a bunch of [classes](http://basscss.com/) that apply styles in a browser-compatible way, has affordances for responsiveness and alleviates the need for inline styles or LESS/CSS files.

With the above 4 tools and following the React paradigm, you shouldn't need CSS/LESS files. IF there are special occasions where you do, these is a `all.less` file, but this is a solution of last resort. Use it sparingly.

### Clean

```bash
yarn clean
```

### Lint

```bash
yarn lint
```

### Prettier

Run from the monorepo root directory:

```
yarn prettier
```

### Resources

##### Toolkit

-   [Styled Components](https://www.styled-components.com/)
-   [BassCSS](http://basscss.com/)

##### Recommended Atom packages:

-   [atom-typescript](https://atom.io/packages/atom-typescript)
-   [linter-tslint](https://atom.io/packages/linter-tslint)
