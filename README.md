# github-style

This is a fork from [github-style](https://github.com/MeiK2333/github-style).
For more information about how to use, please follow the original repo.

> In this repo, there's only list of additional features.
>
> BTW, Documentation in progress🏃‍♂️

## Quick guide

### New features in this fork version:
1. [Pinned posts and recent posts show together](README.md#pinned-posts-and-recent-posts-show-together)
2. [Support reading time estimation](/README.md#support-reading-time-estimation)
3. [Display your real github followers stats](/README.md#display-your-real-github-followers-stats)
4. [Add sponsor link button](/README.md#add-sponsor-link-button)

> Documentation in progress
> 
> 5. [Local search](/README.md#local-search)
> 
> 6. [Show the specific day posts when click the specific block in yearly-contributions graph](/README.md#show-the-specific-day-posts-when-click-the-specific-block-in-yearly-contributions-graph)
> 
> 7. [Support custom css file](/README.md#support-custom-css-file)
> 
> 8. [Support paginator in post page](/README.md#support-paginator-in-post-page)

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

> Since the original repo only display **Pinned** or **Recent** block. In other word, if you set `pin: true` in any of your posts, then there's only display **Pinned** block in your overview page.
>
> However, I want show both in my overview page. In this version, **Pinned** block will show over the **Recent**(_posts here sort by created time_) block. It means they will display together.

![2022-09-02_10-15](https://user-images.githubusercontent.com/32745146/188045141-12f720d0-bb7e-4383-8cca-675be98692d7.png)

### Support reading time estimation

> This feature evaluates the reading time of every post and shows next of the count of words.
>
> The evaluation formula referenced [here](https://kodify.net/hugo/strings/reading-time-text/).

![2022-09-02_10-26](https://user-images.githubusercontent.com/32745146/188046079-2c001f05-7e83-420b-8fd3-f810c28284d0.png)

### Display your real github followers stats

> To show real github followers count, please set `enableGithubFollowers = true` and your github account like `github = kurt-liao` in **config.toml** file.
You can copy the [template](/config.template.toml) in this repo.

![2022-09-02_10-37](https://user-images.githubusercontent.com/32745146/188046956-9af786fd-ccae-4c37-acc1-1a127ac0b9d1.png)

### Add sponsor link button

> Set your sponsor link in **config.toml** like `sponsorLink = "https://www.buymeacoffee.com/vermouth02D"` and the button will show on the page.
> For me, I put the [buymeacoffee](https://www.buymeacoffee.com/) link.

![2022-09-02_10-39](https://user-images.githubusercontent.com/32745146/188047984-c40e8bb7-9af5-4601-b613-d636d5a81415.png)

### Local search

### Show the specific day posts when click the specific block in yearly-contributions graph

### Support custom css file

### Support paginator in post page


## Config Example

@see [config.template.toml](/config.template.toml)
