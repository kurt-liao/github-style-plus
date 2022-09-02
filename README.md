# github-style

This is a fork from [github-style](https://github.com/MeiK2333/github-style).
For more information about how to use, please follow the original repo.

> In this repo, there's only list of additional features.
>
> BTW, Documentation in progress🏃‍♂️

## Quick guide

New features in this fork version:
1. [Pinned posts and recent posts show together](README.md#pinned-posts-and-recent-posts-show-together)
2. [Support reading time estimation](/README.md#support-reading-time-estimation)
3. [Display your real github followers stats](/README.md#display-your-real-github-followers-stats)
4. [Show the specific day posts when click the specific block in yearly-contributions graph](/README.md#show-the-specific-day-posts-when-click-the-specific-block-in-yearly-contributions-graph)
5. [Add sponsor link button](/README.md#add-sponsor-link-button)
6. [Support custom css file](/README.md#support-custom-css-file)
7. [Support paginator in post page](/README.md#support-paginator-in-post-page)

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

## New features✨

### Pinned posts and recent posts show together

### Support reading time estimation

### Display your real github followers stats

### Show the specific day posts when click the specific block in yearly-contributions graph

### Add sponsor link button

### Support custom css file

### Support paginator in post page


## Config Example

@see [config.template.toml](/config.template.toml)
