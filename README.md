# compileMD

## Brief introduction
Markdown files are a popular format for technical project documentation, but as the amount of docu grows, the files can become long and difficult to manage. The solution to this problem is to break down the markdown file into smaller, more manageable seperate `.md` files and then compile them into a single file i.e., `README.md`. Hence, `compileMD` tries to solve this problem.

<b>compileMD compile markdown files into the single README.md.</b>

## Installation
```bash
$ pip3 install --user compileMD
```

## How to use `compileMD`?

For simplicity, create the following folders and files:

```bash
$ mkdir testing
[ testing]$ mkdir md_docs
```

```
[ md_docs]$ vi 00_intro.md

# Project Title
A brief description of what this project does and who it's for.
```

```
[ md_docs]$ vi 01_installation.md

## Installation
Install my-project with npm ...
```

Now, run compileMD:

```
[ testing]$ compileMD
[info] Compiling 00_intro.md into ./README.md
[info] Compiling 01_installation.md into ./README.md
```

`testing` tree looks like this:
```
.
├── md_docs
│   ├── 00_intro.md
│   ├── 01_installation.md
└── README.md
```


## Related
Here are some related links for this repo:
- [https://pypi.org/project/compileMD](https://pypi.org/project/compileMD)
- [Article > How to publish a PIP package?](https://amaharjan.de/how-to-publish-a-pip-package/)
- [Original/first article](https://github.com/asis2016/amaharjande/tree/main/organize-markdown-with-python)


## Contributing
Contributions are always welcome! Please contact hello@amaharjan.de.

## License
[MIT](./LICENSE)









  