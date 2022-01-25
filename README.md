# Steps to use TailwindCSS using only Hugo Pipes

1. Make sure you have these npm dependencies installed
 * Hugo v0.92.0 (May work with older versions too, but not tested)
 * tailwindcss
 * postcss
 * postcss-cli
 * autoprefixer

2. Run `npx tailwindcss init -p` to create a TailwindCSS and a PostCSS config file.
3. Add this to your tailwind.config.js file:
```javascript
   {
        content: ['./layouts/**/*.html', './content/**/*.md']
   }
```
4. Run `hugo` or `hugo server -D --watch` to see the result

Read the full article here: https://dev.to/jonas_duri/how-to-use-tailwindcss-30-without-external-npm-scripts-just-hugo-pipes-2lg9  
This already includes the proposed changes from @nnooney: https://github.com/gohugoio/hugo/issues/8343#issuecomment-1013956389
