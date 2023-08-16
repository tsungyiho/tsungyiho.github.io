# Tsung-Yi Ho
The website is generated using Jekyll, and is hosted at [https://tsungyiho.github.io/](https://tsungyiho.github.io/).

## Table of Contents
- [Build the Website Locally](#build-the-website-locally)
  * [I. Prerequisites](#i-prerequisites)
    + [Step 1: Install Homebrew](#step-1--install-homebrew)
    + [Step 2: Install chruby and the latest Ruby with ruby-install](#step-2--install-chruby-and-the-latest-ruby-with-ruby-install)
    + [Step 3: Install Jekyll and Bundler gems.](#step-3--install-jekyll-and-bundler-gems)
  * [II. Build the Website](#ii-build-the-website)
    + [Step 1: Build the site and make it available on a local server](#step-1--build-the-site-and-make-it-available-on-a-local-server)
    + [Step 2: Browse the website](#step-2--browse-the-website)
- [Update and Maintenance](#update-and-maintenance)
  * [I. Update Bio/Photo/Contact/Social Link](#i-update-bio-photo-contact-social-link)
  * [II. Update Honors](#ii-update-honors)
  * [III. Update Publications](#iii-update-publications)
  * [IV. Update Research Group](#iv-update-research-group)


## Build the Website Locally
### I. Prerequisites
#### Step 1: Install Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### Step 2: Install chruby and the latest Ruby with ruby-install
Install ```chruby``` and ```ruby-install``` with Homebrew:
```bash
brew install chruby ruby-install xz
```

Install the latest stable version of Ruby (supported by Jekyll):
```bash
ruby-install ruby 3.1.3
```

This will take a few minutes, and once it’s done, configure your shell to automatically use ```chruby```:
```bash
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version
```
If you’re using Bash, replace ```.zshrc``` with ```.bash_profile```.

Quit and relaunch Terminal, then check that everything is working:
```bash
ruby -v
```
#### Step 3: Install Jekyll and Bundler gems.
After installing Ruby with ```chruby```, install the latest Jekyll and Bundler gem:
```bash
gem install jekyll bundler
```

### II. Build the Website
#### Step 1: Build the site and make it available on a local server
```bash
bundle exec jekyll serve
```

#### Step 2: Browse the website
Check out your website locally at: [http://localhost:4000](http://localhost:4000).

## Update and Maintenance
### I. Update Bio/Photo/Contact/Social Link
Please check out [_pages/about.md](_pages/about.md).

To update news, please update ([assets/recent_events.tsv](assets/recent_events.tsv)).

### II. Update Honors
Please check out [_pages/honors.md](_pages/honors.md).

### III. Update Publications
This is generated using bibtex retrieved from DBLP. Please update or replace [_bibliography/papers.bib](_bibliography/papers.bib) with the latest one [https://dblp.org/pid/63/4181.bib?param=0](https://dblp.org/pid/63/4181.bib?param=0).

### IV. Update Research Group
Please check out [_pages/research-group.md](_pages/research-group.md).
