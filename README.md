# Gixx-web Static Website 

This is the Jekyll and architecture source code of the [gixx-web.com](https://www.gixx-web.com) website. 

## 1. License

The writings under the [_posts](_posts) folder and the image assets are protected by copyright, the rest is free for learning and using.

## 2. Installation

The installation is pretty straightforward, you need only a little pre-check to generate 

### 2.1. Check Ruby

Make sure you have Ruby 2.1.0 or higher installed

```
$ ruby --version
> ruby 2.x.x
```

If you don't have Ruby installed, [follow the instructions](https://www.ruby-lang.org/en/downloads/).

### 2.2. Install required libraries

#### 2.2.1. GSL

The GSL library provides a wide range of mathematical routines such as random number generators, special functions and least-squares fitting.

**OSX**
```
brew install gsl
```

**Linux / Windows WSL**
```
sudo apt-get install libgsl0ldbl
```
or
```
sudo apt-get install libgsl-dev
```

#### 2.2.2. ImageMagick

The ImageMagick is required for modifying image assets for the responsive design.

**OSX**
```
brew install imagemagick@6
brew install pkg-config
export PATH="/usr/local/opt/imagemagick@6/bin:$PATH"
brew link --force imagemagick@6
```

**Linux / Windows WSL**
```
sudo apt-get install imagemagick libmagickwand-dev pkg-config
```

### 2.3. Install GEM stuffs

```
sudo gem install jekyll
sudo gem install bundler
sudo gem install gsl
sudo gem install rmagick
```

### 2.4. Setup

Simply run the following command in the terminal:

```
bundle install
```

There should be no problem.

## 3. Run

The fun part starts now... After the design is ready, and there are some contents as well, it's time to check it in the browser:

```
jekyll serve -w
```

Then if there's no error, check the site [in the browser](http://127.0.0.1:4000/)

