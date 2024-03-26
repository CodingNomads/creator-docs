# Contributing Workflow

**Do not edit/update/commit directly to the main branch**

The content repositories reflects what's on the platform as of the last commit to `main` or `master`.

## Making Contributions

If you have any contributions you'd like to make, please create a branch, make your changes, and submit a pull request. We'll review it and merge it if it looks good.

If you have small typos or errors that would be quick to fix, you can create a pull request, but you also let us know directly by reaching out via Discord or creating an issue in the repository.

If you have any other questions, or proposals for larger changes, feel free to create an issue in the repository to kick off a discussion.

### Project Structure

We use an exporting tool to create a directory structure with markdown files which is what you see here. The way the course is structured is as follows:

```
Course_Name
│   index.md
│   001_1_section_1
│   │   index.md
│   │   001_lesson.md
│   │   002_lesson.md
│   │   ...
│   002_2_section_2
│   │   index.md
│   │   001_lesson.md
│   │   002_lesson.md
│   │   ...
│   ...
...

```

Everything outside the `Course_Name` folder doesn't get included on the platform. I.e. this document, the `README.md`, doesn't get included. Feel free to add any other files or folders you need to help manage the course content or provide additional resources for instructors.

The first three numbers and underscore (`001_`) on the sections and lessons are there to keep them in order in the file system. They are added by the exporting tool and aren't included in the course content on the platform. That's why it may seem redundant to have `001_1...` and `002_2...` in the folder names, but it's the way that the export tool ensures that the files are in the same order as what appears in the platform.

### YAML Front Matter Metadata

All markdown files have metadata at the top of the file in the form of a YAML front matter block. YAML front matter is a convention to add metadata to markdown files in [YAML format](https://yaml.org/) between two sets of three dashes `---` at the top of the file. Here's an example of what it looks like:

```markdown
---
title: "Lesson Title"
description: "A description of the lesson"
...

---

Lesson content goes here...
```

In general you don't need to touch the metadata, but you may want to adjust a title or description to better fit the content of the lesson, in which case you can do so in the front matter.

**Don't touch other parts of the front matter unless you know what you're doing.**

Since the title is declared in the front matter, don't add an `h1` (`#`) at the top of the markdown file. The title will be automatically added to the page by the platform. Start the content with a brief introduction and then start the headings with `h2` tags (`##`).

### Index Files

The course folder has an `index.md` file which only has front matter and has the course metadata. This metadata has information like the course title, the description, the course image, the course duration, and more. Each section also has a similar `index.md` file.

### Adding a New Lesson

If you want to add a new lesson, you can do so by creating a new markdown file in the appropriate section folder. All you need to add in terms of front matter is `slug`, `title`, `metaTitle`, `description`, `metaDescription`, and `keywords` and `type`.

Since the lessons are numbered, to get your lesson to show up in the right order, you can add another number to the numbering system. Since this is a file system, assume alphabetical order.

- `001`
- `002`
- `003`
- `0033`
- `004`
- `005`
- ...

For example, if you're adding a lesson between `005_` and `006_`, you could name your file `0055_New Lesson Title.md`.

## Historical Releases

For historical purposes, the content repos also contains three releases (so far):

- **Legacy Platform Content**: The content as it was last published on the legacy platform (Moodle).
- **SEO Migration Content**: The content as it was updated in preparation for publish on the new platform.
- **Initial Course Export Content**: The content exported from the new platform as it existed post-initial-publish.
