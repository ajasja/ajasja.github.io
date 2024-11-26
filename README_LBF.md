# How to edit this website

Below a very short intro on how to modify the content of our new website, which is now redirected from  [Github](https://ajasja.github.io) to our domain [...](...).

Some of the pages use the content specified directly within the `.md` **files** in the `_pages` directory:

* *about*
* *contact*

To edit these, simply modify the text using the markdown styling (for basic instructions, see `/pages/markdown.md`) or `html`. The header within the `--` symbols contains the metadata used to generate the page, so don't modify that.

Other pages are generated from individual files within the relevant **folders**:

* *_news*
* *_research*
* *_team*
* *_publications*
* *_software*

To edit those, do the following:

1. If creating a new entry (person, project, publication etc.), copy one of the existing files and rename it.
2. Open the selected `.md` file with *Notepad*, *Notepad++*, *Visual Studio Code* or any other text editor.
3. Modify the metadata in the header within `--` as necessary.
4. Adapt the content below `--` using markdown styling.
5. Do not modify the content within curly brackets `{ }` - this is part of the code that generates pages.
6. Upload the files with your edits into the relevant folder on Nextcloud.
7. For now, you unfortunately cannot see the end result directly. Please let me (Iztok:) know about your edits and I will pull them to github to show online. 

I hope this helps, otherwise please ask.


## Navigation bar
To add sidebar navigation, add the following to the page:
```yml
sidebar:
  nav: "Research"
```
Additionally, in the `_data/navigation.yml` file, add:
```yml
Research:
  - title: Research
    url: /research
    children: 
    - title: First section.
      url: /research#first-section
```
In the page, you can create headings by underlining the heading:
```md
This is a Title
---------
```
This will create a new heading `<h2>` with `id="this-is-a-title"`. This is the anchor you should refer to in the Navigation after the hashtag sign.