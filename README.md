# SubstackSaver - A Fork of Substack2Markdown

This project is a fork of the great tool - [Substack2Markdown](https://github.com/timf34/Substack2Markdown) by [timf34](https://github.com/timf34).

This fork was created to make a better version of this simple CLI tool, add features like images saving, improve links in Markdown files, provide a different approach to authentification on Substack for paid access and many other.

For the original project, please see: [Substack2Markdown](https://github.com/timf34/Substack2Markdown)

## Key Changes in This Fork:

Tracked in [CHANGELOG.md](CHANGELOG.md)

## TODO

- [ ] Add logging
- [ ] Introduce WORK_DIR and EXPORT_DIR Options
- [ ] Implement retry logic
- [ ] Implement reference-style links (improve Markdown readability and maintenance) 
- [ ] Alternative to Selenium for authentification to Substack
- [ ] Add support for downloading images and other media
- [ ] Add tests
- [ ] Add CI
- [ ] Improve documentation

SubstackSaver is a Python CLI tool for downloading free and paid Substack posts and saving them as both Markdown and HTML files, it can generate a simple HTML index page to browse and sort through the posts. It will save paid content as long as you're a paying subscriber of that substack. 


![SubstackSaver Interface](./assets/images/screenshot.png)

Once you run the script, it will create a folder named after the substack in `/substack_md_files`,
and then begin to scrape the substack URL, converting the blog posts into markdown files. Once all the posts hav been saved, it will generate an HTML file in `/substack_html_pages` directory that allows you to browse the posts.

## Features

- Converts Substack posts into Markdown and HTML files.
- Generates HTML index file to browse Markdown files.
- Supports free and paid content (with valid subscription).
- The HTML interface allows sorting essays by date or likes.

## Installation

Clone the repo and install the dependencies:

```bash
# git clone https://github.com/den0k/SubstackSaver.git
# cd SubstackSaver

# # Optinally create a virtual environment
# python -m venv venv
# # Activate the virtual environment
# source venv/bin/activate 

# # then use `pip` to install dependecies

# pip install -r requirements.txt
```

## Usage

Specify the Substack URL and the directory to save the posts to:

```bash
python substack_saver.py
```

## Contact

For any issues/suggestions check the [Issues](https://github.com/den0k/substacksaver/issues) tab. For all other requests (e.g. you want me to create something custom made for you, etc.), you can reach out on directly.
