# RL4AA'25 Website

This is the repository for the website of the 3rd RL4AA workshop (RL4AA'25) to be held at DESY in Hamburg on 2-4 April 2025.

## View the website offline

To view the website offline, you must have [Hugo](https://gohugo.io/) installed. You may follow the [official installation instructions](https://gohugo.io/installation/).

In general, the easiest installation method is to use the package manager of your operating system. On **macOS**, you can use [Homebrew](https://brew.sh/):

```bash
brew install hugo
```

On **Linux**, you can use `apt`:

```bash
sudo apt install hugo
```

On **Windows**, you can use [Winget](https://docs.microsoft.com/en-us/windows/package-manager/winget/):

```bash
winget install Hugo.Hugo.Extended
```

Once you have Hugo installed, you can clone this repository and run the following command in the repository's root directory:

```bash
hugo server
```

This will start a local web server that you can access in your browser at [`http://localhost:1313/RL4AA25/`](http://localhost:1313/RL4AA25/).

## Editing content

For simple content editing, simply edit the Markdown files for the different subpages in the `content/` directory. The content is written in Markdown, which is a simple markup language that is easy to learn. You can find a guide to Markdown [here](https://www.markdownguide.org/).

Images and other files can be found and placed in the `assets/` directory.

Commands of the form `{{< ... >}}` are Hugo shortcodes. They are used as easy-to-use commands for inserting fancy content. Just follow the existing shortcodes in the Markdown files to see how they are used. They typically have arguments of the form `key=value` separated by spaces. Note that there are some shortcodes that enclose longer content. They follow the form

```markdown
{{< shortcode >}}
Some content
{{< /shortcode >}}
```

For more advanced editing, you may need to edit the HTML or CSS files in the `layouts/` directory. This is only necessary if you want to change the layout of the website or add new features.

To view your changes locally, simply save the files. If `hugo server` is running, the changes will automatically update in your browser. When you push your changes to the remote repository, the public website will be updated automatically (provided the deployment is enabled).

## Toggle website public/private

To set the website to public, go to the repository settings, then the "Pages" section, set the "Branch" to `gh-pages` and click "Save". The website will be available at [`https://rl4aa.github.io/RL4AA25/`](https://rl4aa.github.io/RL4AA25/).

To set the website to private, go to the repository settings, then the "Pages" section, set the "Branch" to `None` and click "Save". The website will no longer be available.
