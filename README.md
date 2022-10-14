# github-style

This is a fork from [github-style](https://github.com/MeiK2333/github-style) with some additional features that I've made.

> In this repo, there's only list of additional features.
> For more information about basic usage, please follow the original repo.
> 
> BTW, Documentation is in progress🏃‍♂️

## Quick guide

### New features in this fork version:

1. [Pinned posts and recent posts show together](README.md#-pinned-posts-and-recent-posts-show-together)
2. [Support reading time estimation](/README.md#-support-reading-time-estimation)
3. [Display your real github followers stats](/README.md#-display-your-real-github-followers-stats)
4. [Add sponsor link button](/README.md#%EF%B8%8F-add-sponsor-link-button)
5. [Keyword search locally](/README.md#-keyword-search-locally)
6. [Clickable day contributions](/README.md#-clickable-day-contributions)

> Documentation in progress
>
> 7. [Show the specific day posts when click the specific block in yearly-contributions graph](/README.md#-show-the-specific-day-posts-when-click-the-specific-block-in-yearly-contributions-graph)
>
> 8. [Support custom css file](/README.md#-support-custom-css-file)
>
> 9. [Support paginator in post page](/README.md#-support-paginator-in-post-page)

## Demo

First, take a look at my [personal blog](https://blog.kurtstories.com/), it's the completely demo for this theme.

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

### 📌 Pinned posts and recent posts show together

> Since the original repo only display **Pinned** or **Recent** block. In other word, if you set `pin: true` in any of your posts, then there's only display **Pinned** block in your overview page.
>
> However, I want show both in my overview page. In this version, **Pinned** block will show over the **Recent**(_posts here sort by created time_) block. It means they will display together.

![2022-09-02_10-15](https://user-images.githubusercontent.com/32745146/188045141-12f720d0-bb7e-4383-8cca-675be98692d7.png)

### ⏳ Support reading time estimation

> This feature evaluates the reading time of every post and shows next of the count of words.
>
> The evaluation formula referenced [here](https://kodify.net/hugo/strings/reading-time-text/).

![2022-09-02_10-26](https://user-images.githubusercontent.com/32745146/188046079-2c001f05-7e83-420b-8fd3-f810c28284d0.png)

### 🚶🚶🚶 Display your real github followers stats

> To show real github followers count, please set `enableGithubFollowers = true` and your github account like `github = kurt-liao` in **config.toml** file.
> You can copy the [template](/config.template.toml) in this repo.

![2022-09-02_10-37](https://user-images.githubusercontent.com/32745146/188046956-9af786fd-ccae-4c37-acc1-1a127ac0b9d1.png)

### ❤️ Add sponsor link button

> Set your sponsor link in **config.toml** like `sponsorLink = "https://www.buymeacoffee.com/vermouth02D"` and the button will show on the page.
>
> For me, I put the [buymeacoffee](https://www.buymeacoffee.com/vermouth02D) link.

![2022-09-02_10-39](https://user-images.githubusercontent.com/32745146/188047984-c40e8bb7-9af5-4601-b613-d636d5a81415.png)

### 🔎 Keyword search locally

> Searching in personal site might be important with a growing number of articles, so I've done it.
>
> This feature uses hugo rss that generate `index.xml` feed file, so make sure you have set `params.rss = true`
>
> Though somebody might not want to use this feature, there's another parameter you need to set to true to enable: `params.enableLocalSearch = true`

![](https://i.imgur.com/vKrgR1E.png)

![ezgif com-gif-maker](https://user-images.githubusercontent.com/32745146/187828206-829830a4-3fac-40e3-8bcb-399a98b01680.gif)

### Clickable day contributions

Make yearly-contributions graph clickable like github does. When you click on specific day, it will show you the posts added that day.

![Clickable day contributions](https://i.imgur.com/pSJi4KB.gif)

### 🤲 Show the specific day posts when click the specific block in yearly-contributions graph

### 💡 Support custom css file

### 📟 Support paginator in post page

## Config Example

@see [config.template.toml](/config.template.toml)
