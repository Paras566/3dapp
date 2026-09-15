# 3D Apps — Interactive Beverage Showcase

A browser-based 3D website built with **X3DOM** and **Bootstrap 5** that lets users rotate, zoom, and animate 3D models of Coca-Cola, Sprite, and Dr Pepper bottles. Built as a postgraduate assignment for the 3D Applications module (MSc Advanced Computer Science, University of Sussex).

**Live demo:** https://paras566.github.io/3dapp/assignment/index.html

## Features

- Interactive 3D bottle viewers (rotate/pan/zoom, animation controls) rendered with [X3DOM](https://www.x3dom.org/)
- Custom 3D models authored in Blender / Cinema 4D and exported to X3D, with hand-applied textures
- Responsive multi-page layout (Home, Coca-Cola, Sprite, Dr Pepper) using Bootstrap 5
- No build step or dependencies to install — pure static HTML/CSS/JS

## Tech Stack

- HTML5 / CSS3 / vanilla JavaScript
- [X3DOM](https://www.x3dom.org/) for declarative 3D rendering in the browser
- [Bootstrap 5](https://getbootstrap.com/) for layout and UI components
- 3D models authored in Blender and Cinema 4D

## Project Structure

```
assignment/
├── index.html          # Landing page
├── coke.html            # Coca-Cola 3D viewer
├── sprite.html          # Sprite 3D viewer
├── drpeper.html         # Dr Pepper 3D viewer
├── css/                 # Stylesheets (site + x3dom)
├── js/                  # x3dom.js runtime
├── assets/              # Images and X3D/texture assets used by the pages
└── models/              # Source 3D models (Blender/Cinema 4D) and their X3D exports
```

## Running Locally

Since the site is static, just serve the `assignment` folder with any local web server (opening `index.html` directly can block X3D asset loading due to browser file:// restrictions):

```bash
cd assignment
npx serve .
# or: python -m http.server 8000
```

Then open `http://localhost:8000` (or the port shown) in your browser.
