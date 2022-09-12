# React 3

## Nextjs

Assets - Next.js can serve images under top-level of the public directory. Nextjs can optimize images on-demand. The benefit is that it will not effect the speed of your page. As your scrolling images are then loaded.

`import Image from 'next/image';`

`const YourComponent = () => (`
  `<Image`
    `src="/images/profile.jpg" // Route of the image file`
    `height={144} // Desired size with correct aspect ratio`
    `width={144} // Desired size with correct aspect ratio`
    `alt="Your Name"`
  `/>
);`

Metadata - You can change the metadata within the `Head` tag in a Next.Js page. Make sure to import the Head from 'next/head', then update the export.

`import Head from 'next/head';`

`export default function FirstPost() {`
  `return (`
   ` <>`
      `<Head>`
        `<title>First Post</title>`
      `</Head>`
      `<h1>First Post</h1>`
      `<h2>`
        `<Link href="/">`
          `<a>Back to home</a>`
        `</Link>`
      `</h2>`
    `</>`
  );
}

CSS Styling - Using Css modules it allows the developer to locally scope css the component-level and create unique class names. You can reuse the same Css class name in another file. You can style you pages using Sass, Post Css like Tailwind or CSS in JS.