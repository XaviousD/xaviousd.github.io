---
layout: post
title: Documentation - Jekyll Chirpy and ImageGallery
date: 2022-6-16 12:50:00 -500
categories: [homelab,documentation]
tags: [github,Jekyll,ggreer]
pin: true
---

# Jekyll with Chirpy theme Image Gallery process

Found an image gallery plugin I\'m going to attempt to add into my Jekyll setup that uses the Chirpy theme.  I have NO CLUE how to do this but hopefully with some help from iLude later, I\'ll be able to document that process below.

Hopefully others who have taken on the [#100DaysofHomelab](https://100daysofhomelab.com/) challenge and used TechnoTim\'s [Meet Jekyll](https://techno-tim.github.io/posts/jekyll-docs-site/) video to do their own blog will find this helpfull

More to Come...
<br>

## Update

With the help of iLude, jacobs, projectdp and Thunderfoot from TechnoTim\'s i\'ve managed to integrate ggreer\'s [jekyll-gallery-generator](https://github.com/ggreer/jekyll-gallery-generator) into my jekyll-chirpy setup.  To be honest, I was scarred but it was a rather painless process.  Below are the steps we did to complete this.
<br>

## Step 1

Install the jekyll-gallery-generator gem by adding the below to your Gemfile and running bundle.
```yml
# ggreer Image-Gallery-Generator 
gem 'jekyll-gallery-generator'
```

Install dependencies on Ubuntu
```bash
sudo apt-get install libmagickwand-dev
```
Install the Gem Package
```bash
bundle install
```

Create the Directory Structure within your site.  This is in the root folder, photos<br>
*you will be able to access this directly via the following:  http://websiteurl/folder* <br>
My example is below:
```bash
mkdir photos
mkdir photos/ImageDirectory1
mkdir photos/ImageDirectory2
```

Build/Run local instance of Jekyll
```bash
bundle exec jekyll s
```

This plugin reads several config options from _config.yml. The following options are supported (default settings are shown):<br>
This information comes directly from ggreer's [jekyll-gallery-generator](https://github.com/ggreer/jekyll-gallery-generator) github.
```yml
gallery:
  dir: photos               # Path to the gallery
  symlink: false            # false: copy images into _site. true: create symbolic links (saves disk space)
  title: "Photos"           # Title for gallery index page
  title_prefix: "Photos: "  # Title prefix for gallery pages. Gallery title = title_prefix + gallery_name
  sort_field: "date_time"   # How to sort galleries on the index page.
                            # Possible values are: title, date_time, best_image
  thumbnail_size:
    x: 400                  # max width of thumbnails (in pixels)
    y: 400                  # max height of thumbnails (in pixels)
  # The following options are for individual galleries.
  galleries:
    gallery_1: # Subfilder that is set via the above dir: photos option
      best_image: IMG_1068.JPG  # The image to show on the gallery index page. Defaults to the last image.
    gallery_2:
      best_image: IMG_0690.JPG
      name: "日本の旅"       # Defaults to directory name, replacing _ with spaces & capitalizing words.
    awesome_stuff:
      best_image: snaileo_gonzales.jpg
      sort_reverse: true    # Reverse sort images in gallery.
    secret_stuff:
      hidden: true          # Don't show this gallery on the index page. People must guess the URL.
    with_info:
      info:
        desc: "Gallery Description" # Info fields can be used in custom templates.
```
