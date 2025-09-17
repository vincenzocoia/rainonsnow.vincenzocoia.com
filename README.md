[![Netlify Status](https://api.netlify.com/api/v1/badges/f6fa3c46-7a3c-4641-abb1-7155c04a3e2f/deploy-status)](https://app.netlify.com/projects/rainonsnow/deploys)

# ESA OSIP project website

This website uses Hugo Blox to generate a static website, which is hosted on Netlify. It uses two themes, Academic CV and Landing Page, so that it can incorporate a larger collection of blocks.

### Generating Publications

Generate from bibtex file -- update `content/publications.bib`.

I use [academic-file-converter](https://github.com/GetRD/academic-file-converter) to convert each bibtex entry to `content/publication/ENTRY` (as recommended by Hugo Blox):

1. Navigate to `content/` in terminal.
2. Execute the following commands:

```
academic import publications.bib publication/ --featured
```

3. Edit the `index.md` markdown for each new publication folder that gets created to make sure there's no boilerplate.
	- Last time, had to get rid of the boilerplate "Add the **full text** or **supplementary notes** for the publication here using Markdown formatting."

Notes: 

- The `--overwrite` tag will overwrite existing output folders. But this workflow was never intended to be fully reproducible, because of the manual edits that are sometimes required in the index files.

## Hugo Blox Links

Documentation: https://docs.hugoblox.com/

Themes on github:

- Landing page theme: 
	- GitHub: https://github.com/HugoBlox/theme-landing-page
	- Demo page: https://theme-landing-page.netlify.app/
- Academic CV theme: 
	- GitHub: https://github.com/HugoBlox/theme-academic-cv
	- Demo page: https://academic-demo.netlify.app/

List of all templates: https://hugoblox.com/templates/ 