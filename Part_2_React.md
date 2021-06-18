# Part 2 - React.js

## [Learning JS Together - React (#2)](https://www.youtube.com/watch?v=7hC0HpkBw8g)

📺 YouTube Live: <https://youtu.be/7hC0HpkBw8g>

---

Hacking Kintone Plug-in with React!

We will be converting a jQuery-based Kintone Plug-in to a React version.
Specifically, we will be focusing on the Plug-in's `config` settings page in this episode.

Steps:
1. [Create React App](https://create-react-app.dev/)
2. Simplifying the boilerplate code
3. Getting the original settings page code
4. Setup HTML Rendering
5. `npm run build`

---

## Notes

### Starting Point

[Table-Utility-Plug-in/blob/main/1_Starting_Point/src/js/config.js](https://github.com/ahandsel/Table-Utility-Plug-in/blob/main/1_Starting_Point/src/js/config.js)

Command to create a sample React App to get you started with a React project

`npx create-react-app`

[Table-Utility-Plug-in/1_Starting_Point/src/css/](https://github.com/ahandsel/Table-Utility-Plug-in/tree/main/1_Starting_Point/src/css)

React.StrictMode is a tool for highlighting potential problems in an application. Strict mode checks are run in development mode only; they do not impact the production build.

[Strict Mode – React](https://reactjs.org/docs/strict-mode.html)

Moved [config.html](https://github.com/ahandsel/Table-Utility-Plug-in/blob/main/1_Starting_Point/src/html/config.html) --> App.js

We want main.[hash].chunk.js after the `npm run build` command

Create React App Doc | Creating a Production Build
<https://create-react-app.dev/docs/production-build/>

How do I add CSS classes to components?
> Pass a string as the className prop

[Styling and CSS – React](https://reactjs.org/docs/faq-styling.html#how-do-i-add-css-classes-to-components)
