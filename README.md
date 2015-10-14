# Ceevee Skeleton for Grav

![Ceevee](assets/readme_1.png)

Ceevee is a clean, modern, fully responsive site template for your resume and portfolio. With this template, you can easily introduce yourself and showcase your works to future clients and employers. Also, it is flexible and easy to customize so you even use this template as a creative, business or portfolio site for your company.

# Built on:

* Bootstrap
* FlexSlider
* Smooth Scroll
* jQuery Waypoints
* Animate.css

# Features:

* HTML5 and CSS3
* Fully Responsive
* Attractive and modern design
* Various templates for presenting your content

## Basic Setup for a new Grav site

The simplest way to install Ceevee theme for Grav is to download and install the Ceevee Skeleton package:

1. [Download Ceevee Skeleton](http://getgrav.org/downloads/skeletons#extras)
2. Simply unzip the package into your web root folder.
3. Point your browser at the folder, job done!

**TIP:** Check out the [general Grav installation instructions](http://learn.getgrav.org/basics/installation) for more details on this process.

---

## Existing Grav site

It is possible to install just the theme, but page content will need to reference the [Ceevee theme](https://github.com/getgrav/grav-theme-ceevee)'s supported templates.  It is strongly advised to at least install the Ceevee Skeleton package to see the theme's capabilities in action.

To install  **just** the theme:

```
$ bin/gpm install ceevee
```

# Configuration
Configuration of Ceevee theme consist of two parts:
* configuration file (from [skeleton](https://github.com/getgrav/grav-skeleton-ceevee-site/commits?author=hexplor)): "user/config/site.yaml"
* header variables (inside markdown files)

In configuration file you can set basic values for header, footer and general.
In markdown files, you can manage page content and overall look of the separate section. For example, below is a portfolio.md header section:

```markdown
portfolio:
  - title: "Creative Minds"
    img: portfolio-01.jpg
    img_text: View More
    img_url: "#"
    content: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultricies nulla non metus pulvinar imperdiet. Praesent non adipiscing libero."
```

In above example you can specify title, image, roll over text, url and content for each separate portfolio element.

Rest of the sections is made in similar approach. Remember to preserve original idenation to avoid issues.


# Credits

### Bootstrap

[Bootstrap](http://getbootstrap.com/) by Twitter. Licensed under [MIT](https://github.com/twbs/bootstrap/blob/master/LICENSE)

### FancyBox

[FancyBox](http://fancyapps.com/fancybox/) by fancyApps. Licensed under [CC BY-NC 3.0](http://creativecommons.org/licenses/by-nc/3.0/)

### FlexSlider

[FlexSlider](http://www.woothemes.com/flexslider/) by WooThemes. Licensed under [GNU GENERAL PUBLIC LICENSE](https://github.com/woothemes/FlexSlider/blob/master/LICENSE.md)

### Waypoints

[Waypoints](https://github.com/imakewebthings/waypoints) by Caleb Troughton. Licensed under [MIT](https://github.com/imakewebthings/waypoints/blog/master/licenses.txt)

### Animate.css

[Animate.css](https://daneden.github.io/animate.css/) by Dan Eden

### Font Awesome Icons

[Font Awesome](http://fortawesome.github.io/Font-Awesome/) by Dave Gandy. Licensed under [MIT](http://opensource.org/licenses/mit-license.html)

## Misc

Follow Pete: [Twitter](https://twitter.com/peterfinlan), [Dribbble](http://www.dribbble.com/peterfinlan), [GitHub](https://github.com/peterfinlan)

Follow Codrops: [Twitter](http://www.twitter.com/codrops), [Facebook](http://www.facebook.com/pages/Codrops/159107397912), [Google+](https://plus.google.com/101095823814290637419), [GitHub](https://github.com/codrops), [Pinterest](http://www.pinterest.com/codrops/)
