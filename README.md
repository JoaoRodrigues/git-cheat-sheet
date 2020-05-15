# Git Cheat Sheet

Feel free to use this cheat sheet for yourself or for teaching workshops. You can see it rendered
as an HTML page [here](https://joaorodrigues.github.io/git-cheat-sheet/) or download it as a PDF
file [here](git-cheat-sheet.pdf).

## Contributing
### Editing the Markdown file.
The cheat sheet is written as a single Markdown file and published as a Github page using the minimal theme. We recommend using [Typora](https://typora.io/) to edit the markdown file locally. 

### Previewing the rendered HTML page
If you want to preview the rendered web page, setup Jekyll using the instructions [on this page](https://help.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll). 

### Previewing the PDF file
The PDF version is automatically generated using [wkhtmltopdf](https://wkhtmltopdf.org/). To preview changes locally, generate the HTML page, install wkhtmltopdf, and then run:

```bash
wkhtmltopdf https://localhost:4000 new.pdf
```

## License
Licensed under CC BY-SA 4.0, for details see [LICENSE.md](LICENSE.md).
