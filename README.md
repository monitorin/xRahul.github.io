## Personalized blog & profile


[![GitHub license](https://img.shields.io/github/license/xRahul/xRahul.github.io.svg?style=flat-square)](https://github.com/xRahul/xRahul.github.io/blob/new-site/LICENSE)
[![Build Status](https://travis-ci.org/xRahul/xRahul.github.io.svg?branch=new-site)](https://travis-ci.org/xRahul/xRahul.github.io)
![imgBot](https://img.shields.io/badge/imgBot-optimized-brightgreen.svg)
![Gem Version](https://img.shields.io/gem/v/jekyll.svg)
[![security](https://hakiri.io/github/xRahul/xRahul.github.io/new-site.svg)](https://hakiri.io/github/xRahul/xRahul.github.io/new-site)
[![libraries.io](https://img.shields.io/librariesio/github/xRahul/xRahul.github.io.svg)](https://libraries.io/github/xRahul/xRahul.github.io)

[![GitHub PageSpeed](https://api.speedbadge.io/v1?url=https://rahulja.in&showStratLabel=true&strat=mobile)](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Frahulja.in%2F&tab=mobile)
[![GitHub PageSpeed](https://api.speedbadge.io/v1?url=https://rahulja.in&showStratLabel=true&strat=desktop)](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Frahulja.in%2F&tab=desktop)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/d251b6435fc844c887ea6c7e58f0c982)](https://www.codacy.com/app/xRahul/xRahul.github.io)
[![Maintainability](https://api.codeclimate.com/v1/badges/f6e013323629b1fc88c2/maintainability)](https://codeclimate.com/github/xRahul/xRahul.github.io/maintainability)
[![CodeFactor](https://www.codefactor.io/repository/github/xrahul/xrahul.github.io/badge)](https://www.codefactor.io/repository/github/xrahul/xrahul.github.io)
[![codebeat badge](https://codebeat.co/badges/eb3cbae9-7f2b-41f1-9b06-0c0966d9a636)](https://codebeat.co/projects/github-com-xrahul-xrahul-github-io-new-site)

#### Home page (List of Posts)
[![Lighthouse Performance score: 94/100](https://lighthouse-badge.appspot.com/?score=94&compact&category=Performance)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in)
[![Lighthouse Accessibility score: 100/100](https://lighthouse-badge.appspot.com/?score=100&compact&category=Accessibility)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in)
[![Lighthouse Best Practices score: 100/100](https://lighthouse-badge.appspot.com/?score=100&compact&category=Best+Practices)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in)
[![Lighthouse SEO score: 100/100](https://lighthouse-badge.appspot.com/?score=100&compact&category=SEO)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in)

#### Article page (Post)
[![Lighthouse Performance score: 66/100](https://lighthouse-badge.appspot.com/?score=66&compact&category=Performance)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in/posts/getting-started-with-gradle-using-java-application)
[![Lighthouse Accessibility score: 93/100](https://lighthouse-badge.appspot.com/?score=93&compact&category=Accessibility)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in/posts/getting-started-with-gradle-using-java-application)
[![Lighthouse Best Practices score: 100/100](https://lighthouse-badge.appspot.com/?score=100&compact&category=Best+Practices)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in/posts/getting-started-with-gradle-using-java-application)
[![Lighthouse SEO score: 96/100](https://lighthouse-badge.appspot.com/?score=96&compact&category=SEO)](https://lighthouse-dot-webdotdevsite.appspot.com/lh/html?url=https://rahulja.in/posts/getting-started-with-gradle-using-java-application)

![Image of rahulja.in](https://github.com/xRahul/xRahul.github.io/raw/new-site/_assets/images/posts/configure-this-site-locally-for-development/og-image%402x.png "rahulja.in")

Install ruby 2.6.5

```bash
rbenv install 2.6.5
rbenv global 2.6.5
ruby -v
```

Install site

```bash
git clone https://github.com/xRahul/xRahul.github.io.git
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=36000'
cd xRahul.github.io/
git branch -r | grep -v '\->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done
git fetch --all
git pull --all

bin/setup
--or--
npm run setup
```

Run local development server

```bash
LC_ALL=en_US.UTF-8 bundle exec jekyll serve --drafts
--or--
npm run local
```

Deploy to github master branch

```bash
bin/deploy
--or--
npm run publish
```
