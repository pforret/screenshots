# screenshots

![](assets/screenshots.jpg)

Automatically make screenshots of all your websites

## Installation 

### Create new repo with this one as template

![img.png](assets/use_template.png)

```bash
# clone the new repo to your local machine
git clone git@github.com:<your username>/<your repo>>.git

# remove all images from the images folder
rm images/*.png

# replace the URLS in sites.txt by your own URLs
echo "https://www.yoursite.com" > sites.txt

# check in the repo with changes
git -a -m "new sites"

# wait until Github Actions have run and created all your screenshots

# now get the updated image files
git pull
```

## Based on

* [github.com/features/actions](https://github.com/features/actions): Github Actions
* [simonw/shot-scraper](https://github.com/simonw/shot-scraper): Playwright based CLI screenshotting - which is based on
* [microsoft/playwright-python](https://github.com/microsoft/playwright-python): Playwright testing and automation library
* [pforret/bashew](https://github.com/pforret/bashew): bash micro-framework