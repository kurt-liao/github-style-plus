# Github Style Plus

This is a fork from [github-style](https://github.com/MeiK2333/github-style) with some additional features that I made.

> In this repo, the documentation only introduce additional features.
> For more information about basic usage, please follow the original repo.

## Quick guide

### New features in this fork version:

1. [Pinned posts and recent posts show together](#pinned-posts-and-recent-posts-show-together)
2. [Support reading time estimation](#support-reading-time-estimation)
3. [Display your real github followers stats](#display-your-real-github-followers-stats)
4. [Add sponsor link button](#add-sponsor-link-button)
5. [Keyword search locally](#keyword-search-locally)
6. [Clickable day contributions](#clickable-day-contributions)
7. [Support custom css file](#support-custom-css-file)
8. [Support previous and next post](#support-previous-and-next-post)
9. [Show more button](#show-more-button)
10. [Update old Google Analytics to GA4](#update-old-google-analytics-to-ga4)
11. [Support GTM Script](#support-gtm-script)
12. [Custom organizations block](#custom-organizations-block)

## Demo

First, take a look at my [blog](https://blog.kurtstories.com/), it's the completely demo for this theme.

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

In the original version, only one of *Pinned* block and *Recent* block will be shown.
In this version, both blocks will display together.

![2022-09-02_10-15](https://user-images.githubusercontent.com/32745146/188045141-12f720d0-bb7e-4383-8cca-675be98692d7.png)
---

### Support reading time estimation

This feature evaluates the reading time of every post and shows the count of words.
>The evaluation formula referenced [here](https://kodify.net/hugo/strings/reading-time-text/).

![2022-09-02_10-26](https://user-images.githubusercontent.com/32745146/188046079-2c001f05-7e83-420b-8fd3-f810c28284d0.png)
---

### Display your real github followers stats

To show real github followers count, please set `enableGithubFollowers = true` and your github account like `github = kurt-liao` in *config.toml* file.

![](https://i.imgur.com/LkBFrVF.jpg)


![](https://i.imgur.com/htrKTFN.jpg)

---

### Add sponsor link button

Set your sponsor link in **config.toml** like `sponsorLink = "https://www.buymeacoffee.com/vermouth02D"` and the button will show on the page.

For me, I put the [buymeacoffee](https://www.buymeacoffee.com/vermouth02D) link.

![2022-09-02_10-39](https://user-images.githubusercontent.com/32745146/188047984-c40e8bb7-9af5-4601-b613-d636d5a81415.png)
---

### Keyword search locally

Searching in personal site might be important with a growing number of articles.
This feature uses hugo rss that generate `index.xml` feed file, so make sure you have set `params.rss = true`
Since somebody might not want to use this feature, there's another parameter you need to set to true to enable: `params.enableLocalSearch = true`

![](https://i.imgur.com/9k70xpQ.jpg)


![ezgif com-gif-maker](https://user-images.githubusercontent.com/32745146/187828206-829830a4-3fac-40e3-8bcb-399a98b01680.gif)
---

### Clickable day contributions

Make yearly-contributions graph clickable like github does. When you click on specific day, it will show you the posts added that day.

![Clickable day contributions](https://i.imgur.com/pSJi4KB.gif)
---

### Support custom css file

If you want to use some custom style, create a style file in **static** folder.
![](https://i.imgur.com/BgbVvrH.jpg)


Then, set file path in *config.toml* file.
![](https://i.imgur.com/tZHHcgL.jpg)

---
### Support previous and next post

![](https://i.imgur.com/RbYKDnS.jpg)

---

### Show more button

For the speed of page loaded in the first paint, I decide to hide most of posts when the page first loaded.
![](https://i.imgur.com/0cGT1Qx.gif)

---

### Update old Google Analytics to GA4

Since the old Google Analytics is being retired. I've change the old GA code to GA4.
![](https://i.imgur.com/bpCFD6N.png)

---

### Support GTM Script

Apart from Google Analytics, we may also want to add GTM Script.
To do this, just add `gtmId = "xxx"` in your *config.toml* file

![](https://i.imgur.com/iEVBm98.jpg)

---

### Custom organizations block

You may want to set some custom organizations except Github, Twitter, Facebook...
Therefore, I've add the custom organization block for you to do so.
The settings in *config.toml* might look like this:

![](https://i.imgur.com/e6sFTIp.png)

And the effect would look like:
![](https://i.imgur.com/4bd3KRx.jpg)

## Config Example

@see [config.template.toml](/config.template.toml)
