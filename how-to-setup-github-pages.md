# How Setup Github Pages

## Table of Content


<!-- TOC -->

- [How Setup Github Pages](#how-setup-github-pages)
  - [Table of Content](#table-of-content)
  - [Step 1: Enable GitHub Pages](#step-1-enable-github-pages)
    - [:keyboard: Activity: Enable GitHub Pages](#keyboard-activity-enable-github-pages)
  - [Step 2: Configure your site](#step-2-configure-your-site)
    - [:keyboard: Activity: Configure your site](#keyboard-activity-configure-your-site)
  - [Step 3: Customize your homepage](#step-3-customize-your-homepage)
    - [:keyboard: Activity: Create your homepage](#keyboard-activity-create-your-homepage)
  - [Step 4: Create a blog post](#step-4-create-a-blog-post)
    - [:keyboard: Activity: Create a blog post](#keyboard-activity-create-a-blog-post)
  - [Step 5: Merge your pull request](#step-5-merge-your-pull-request)
    - [:keyboard: Activity: Merge your changes](#keyboard-activity-merge-your-changes)

<!-- /TOC -->

## Step 1: Enable GitHub Pages

_Welcome to GitHub Pages and Jekyll :tada:!_

The first step is to enable GitHub Pages on this [repository](https://docs.github.com/en/get-started/quickstart/github-glossary#repository). When you enable GitHub Pages on a repository, GitHub takes the content that's on the main branch and publishes a website based on its contents.

### :keyboard: Activity: Enable GitHub Pages

1. Open a new browser tab, and work on the steps in your second tab while you read the instructions in this tab.
1. Under your repository name, click **Settings**.
1. Click **Pages** in the **Code and automation** section.
1. Ensure "Deploy from a branch" is selected from the **Source** drop-down menu, and then select `main` from the **Branch** drop-down menu.
1. Click the **Save** button.
1. Wait about _one minute_ then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
   > Turning on GitHub Pages creates a deployment of your repository. GitHub Actions may take up to a minute to respond while waiting for the deployment. Future steps will be about 20 seconds; this step is slower.
   > **Note**: In the **Pages** of **Settings**, the **Visit site** button will appear at the top. Click the button to see your GitHub Pages site.

## Step 2: Configure your site

_You turned on GitHub Pages! :tada:_

We'll work in a branch, `my-pages`, that I created for you to get this site looking great. :sparkle:

Jekyll uses a file titled `_config.yml` to store settings for your site, your theme, and reusable content like your site title and GitHub handle. You can check out the `_config.yml` file on the **Code** tab of your repository.

We need to use a blog-ready theme. For this activity, we will use a theme named "minima".

### :keyboard: Activity: Configure your site

1. Browse to the `_config.yml` file in the `my-pages` branch.
1. In the upper right corner, open the file editor.
1. Add a `theme:` set to **minima** so it shows in the `_config.yml` file as below:
   ```yml
   theme: jekyll-theme-hacker
   ```
1. (optional) You can modify the other configuration variables such as `title:`, `author:`, and `description:` to further customize your site.
1. Commit your changes.
1. (optional) Create a pull request to view all the changes you'll make throughout this course. Click the **Pull Requests** tab, click **New pull request**, set `base: main` and `compare:my-pages`.
1. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

## Step 3: Customize your homepage

_Nice work setting the theme! :sparkles:_

You can customize your homepage by adding content to either an `index.md` file or the `README.md` file. GitHub Pages first looks for an `index.md` file. Your repository has an `index.md` file so we can update it to include your personalized content.

### :keyboard: Activity: Create your homepage

1. Browse to the `index.md` file in the `my-pages` branch.
1. In the upper right corner, open the file editor.
1. Type the content you want on your homepage. You can use Markdown formatting on this page.
1. (optional) You can also modify `title:` or just ignore it for now. We'll discuss it in the next step.
1. Commit your changes to the `my-pages` branch.
1. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

## Step 4: Create a blog post

_Your home page is looking great! :cowboy_hat_face:_

GitHub Pages uses Jekyll. In Jekyll, we can create a blog by using specially named files and frontmatter. The files must be named `_posts/YYYY-MM-DD-title.md`. You must also include `title` and `date` in your frontmatter.

**What is _frontmatter_?**: The syntax Jekyll files use is called YAML frontmatter. It goes at the top of your file and looks something like this:

```yml
---
title: "Welcome to my blog"
date: 2019-01-20
---
```

For more information about configuring front matter, see the [Jekyll frontmatter documentation](https://jekyllrb.com/docs/frontmatter/).

### :keyboard: Activity: Create a blog post

1. Browse to the `my-pages` branch.
1. Click the `Add file` dropdown menu and then on `Create new file`.
1. Name the file `_posts/YYYY-MM-DD-title.md`.
1. Replace the `YYYY-MM-DD` with today's date, and change the `title` of your first blog post if you'd like.
   > If you do edit the title, make sure there are hyphens between your words.
   > If your blog post date doesn't follow the correct date convention, you'll receive an error and your site won't build. For more information, see "[Page build failed: Invalid post date](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/troubleshooting-jekyll-build-errors-for-github-pages-sites)".
1. Type the following content at the top of your blog post:
   ```yaml
   ---
   title: "YOUR-TITLE"
   date: YYYY-MM-DD
   ---
   ```
1. Replace `YOUR-TITLE` with the title for your blog post.
1. Replace `YYYY-MM-DD` with today's date.
1. Type a quick draft of your blog post. Remember, you can always edit it later.
1. Commit your changes to your branch.
1. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
   
## Step 5: Merge your pull request

_Nice work, friend :heart:! People will be reading your blog in no time!_

You can now [merge](https://docs.github.com/en/get-started/quickstart/github-glossary#merge) your pull request!

### :keyboard: Activity: Merge your changes

1. Merge your changes from `my-pages` into `main`. If you created the pull request in step 2, just open that PR and click on **Merge pull request**. If you did not create the pull request earlier, you can do it now by following the instructions in [step 2](/.github/steps/2-configure-your-site.md).
1. (optional) Delete the branch `my-pages`.
1. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.