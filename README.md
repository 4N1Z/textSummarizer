## Test Summarization Tool

This is a web application that uses the PaLM API to summarize text input by the user. The PaLM API is a language model developed by Google that is capable of generating high-quality summaries of text.

The front end is made with Svelte.
#### Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).  


#### DEVElOPMENT IN PROGRESS !

Requirements
## To locally setup the project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# select the current directory
cd textSummarizer

#  instal dependencies with 
npm install 
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```
## Usage
- Open the index.html file in your web browser.
- Enter the text you want to summarize in the input field.
- Click the "Summarize" button.
- The summarized text will be displayed in the output field.
- You can preview the production build with `npm run preview`.

## Limitations

The PaLM API is a powerful tool, but it has some limitations. In particular, it may not work well with very short or very long texts, and it may not always produce accurate or useful summaries. Additionally, the API has limits on how many requests can be made per month, so this application may not work if those limits are exceeded.

## License
This application is provided under the MIT license. See the `LICENSE` file for more information.

## Acknowledgements
This application was made possible by the PaLM API developed by Google