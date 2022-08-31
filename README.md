# github-style

This is a fork from [github-style](https://github.com/MeiK2333/github-style).
For more information about how to use, please follow the original repo.

> In this repo, there's only list of additional features.
>
> BTW, Documentation in progress🏃‍♂️

## Demo

First, take a look at my [personal blog](https://kurt-liao.github.io/), it's the completely demo for this theme.

## Usage

### Init hugo site

```bash
hugo new site mysite
cd mysite
```

### Install the theme

```bash
git submodule add git@github.com:kurt-liao/github-style-plus.git themes/github-style-plus
```

### Update the theme

If you just installed the theme, it is already in the latest version. If not, you can update using the below commands

```bash
cd themes/github-style-plus
git pull
```

Then, you need to rename the previous `posts` folder to `post`

```bash
cd <you-project-folder>
mv content/posts content/post
```

## config.toml example

@see [config.template.toml](/config.template.toml)
