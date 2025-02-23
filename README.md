# AMISR User Manual

This is the repository hosting all the files used to create the AMISR User Manual, available at https://amisr.github.io/amisr_user_manual

This is intended to be a basic guide to help scientific users access, visualize, and interpret AMISR data.  It is available as a [jupyter book](https://jupyterbook.org/en/stable/intro.html) hosted on [GitHub Pages](https://pages.github.com/). The notebooks included provide examples of some of the more common analysis and plotting tools.  Please feel free to download notebooks if they are useful, or copy/paste examples into your own code and modify as appropriate!

## Contributing
Contributing to this manual is highly encouraged!  Please heed the following guidelines:

### Submit an Issue
If you have a question about some content in the book, think an area needs additional explanation or detail, have a suggestion of new content to add, or find a bug in example code or a broken webpage, please [submit an issue](https://github.com/amisr/amisr_user_manual/issues).  Where appropriate, use the following labels:

- **question:** A question about content in the book or how to use the data correctly
- **content:** Suggestions about modifying existing content or adding new content
- **bug:** Error in a notebook or a broken link or webpage

### Contributing Material
If you have content or examples you would like to contribute to the book, please do!  The following steps are recommended:

1. Fork and clone your own copy of this repository.
```
git clone https://github.com/<your_username>/amisr_user_manual.git
cd amisr_user_manual
```
2. Install the current requirements in your environment.  This can be done from the environment file if you use conda.  If you typically install packages with pip, you will have to open `environment.yml` and manually install the packages listed there.
```
conda env update --name <your_environment_name> --file environment.yml
```
3. Add your content.  This can be in the form of markdown files or jupyter notebooks.  All content files should be contained within the `src` directory and subdirectories within.
4. Add any pages you created to `_toc.yml`.
5. Add any packages your examples rely on to `environment.yml`.  Try to avoid using large packages or anything that may have trouble with a default installation when possible.
6. Add your name and any relevant funding sources under the *Attribution* section in `src/intro.md`.
7. Build the book locally.
```
jupyter-book build .
```
8. Check the local build to make sure your material looks correct.  The build command should have created the file `_build/html/index.html` which can be opened in any browser.
9. Commit your changes.  This can happen at multiple stages as you develop content.
10. Push changes to your local fork on GitHub.
11. Create a pull request from your local branch to the `main` branch of [amisr/amisr_user_manual](https://github.com/amisr/amisr_user_manual).  When the pull request is merged, the webpage will be updated automatically.

Refer to the [jupyter book docs](https://jupyterbook.org/en/stable/intro.html) for more detailed information about syntax and building the book.

