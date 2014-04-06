Title: How to batch convert images in Ubuntu 12.04
Date: 2014-04-04 21:06
Category: Tips
Tags: ubuntu, imagemagick
Slug: how-to-batch-convert-images-in-ubuntu
Author: eddyzhow
Summary:

Install imagemagick :

```
sudo apt-get install libmagickwand-dev imagemagick
```

and then cd to your directory and run :

```
for file in *.jpg ; do convert "$file[144x]" "./thumbs/${file/%jpg/png}" ; done
```
