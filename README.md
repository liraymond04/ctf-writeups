# ctf-writeups

Repository of writeups for Capture the Flag (CTF) challenges

## Remote loading

`files.yaml` defined in the root directory is used for detailing how to remote load the repo for my [personal site](https://github.com/liraymond04/personal-site)'s markdown blog, and makes it easy to fetch and map metadata on all of the repo's files without recursing the entire repo with GitHub's API

The structure of `files.yaml` emulates the file structure of the repository with recursive `directories:` fields, and contains the extra metadata for each markdown file such as tags, keywords, and page type. 

As well, usable file paths for images are implicitly described with `type: image` under entires in the `files:` field
