# Read 39
## React 3

The second page we added currently does not have styling. Let's add some CSS to style the page.

Next.js has built-in support for CSS and Sass. For this course, we will use CSS.

This lesson will also talk about how Next.js handles static assets like images and page metadata like the <title> tag.

What You’ll Learn in This Lesson

In this lesson, you’ll learn:

How to add static files (images, etc) to Next.js.

How to customize what goes inside the <head> for each page.

How to create a reusable React component which is styled using CSS Modules.

How to add global CSS in pages/_app.js.

Some useful tips for styling in Next.js.

Prerequisites

Basic CSS knowledge. This course will go over how to add CSS in a Next.js app, but it won't cover CSS fundamentals.

Download Starter Code (Optional)

If you’re NOT continuing from the previous lesson, you can download, install, and run the starter code for this lesson below. This sets up a nextjs-blog directory such that it’s identical to the result of the previous lesson.

Again, this is NOT necessary if you’ve just finished the previous lesson.

npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn-starter/tree/master/assets-metadata-css-starter"

Then follow the instructions from the command output (cd into the directory and start the development server).

Assets
First, let’s talk about how Next.js handles static assets such as images.

Next.js can serve static files, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

If you open pages/index.js in your application and take a look at the <footer>, we refer to the logo image like so:


The logo image exists inside the public directory at the top level of your application.

The public directory is also useful for robots.txt, Google Site Verification, and any other static assets. Check out the documentation for Static File Serving to learn more.

This page is using a library called styled-jsx. It’s a “CSS-in-JS” library — it lets you write CSS within a React component, and the CSS styles will be scoped (other components won’t be affected).

Next.js has built-in support for styled-jsx, but you can also use other popular CSS-in-JS libraries such as styled-components or emotion.

Furthermore, Next.js’s code splitting feature works on CSS Modules as well. It ensures the minimal amount of CSS is loaded for each page. This results in smaller bundle sizes.

CSS Modules are extracted from the JavaScript bundles at build time and generate .css files that are loaded automatically by Next.js.

This App component is the top-level component which will be common across all the different pages. You can use this App component to keep state when navigating between pages, for example.
