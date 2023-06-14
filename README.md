# What is this?

[Math on GitHub is buggy](https://github.com/nschloe/github-math-bugs). This repository is to provide a bug-free markdown preview with mathematical formulas that may be broken in the original GitHub markdown renderer.

Once this website is deployed, suppose your website is `sub.example.com`, you can view a properly rendered version of a GitHub markdown file. 

For example, suppose a `README.md` file is located in a repository named `blabla`, its path inside this directory is `doc/README.md`, and the owner of this repository is `someone`, you can visit
```
https://sub.example.com?user=someone&repo=blabla&path=doc/README.md
```
and you shall see a properly rendered version.

Note that you should provide a GitHub access token, as this will use the GitHub API to fetch the raw content of the specified markdown file.

# Deploy with netlify

This project can be readily deployed to netlify.

[![Deploy with Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/rk-terence/github-readme-preview#GITHUB_AUTH_TOKEN=)

Please set environment variable `GITHUB_AUTH_TOKEN` to your GitHub access token in your netlify site configuration.