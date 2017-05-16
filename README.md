# Kirby Enhanced Textarea v1.4

This textarea extends the built-in textarea without reinventing the wheel. Handy and customizable headline functions, intelligent list buttons and a custom page selector make editing textareas a breeze.

![Preview](https://cloud.githubusercontent.com/assets/7975568/26103764/44eb2fc4-3a3b-11e7-87dc-86b328f22f85.gif)

## Installation

Download or clone this repository, put the folder into your `site/fields` folder and rename it to `textarea`. Alternatively you can also use the [Kirby CLI](https://github.com/getkirby/cli).

## Configuration

### Headlines

You can change the headline buttons to any headline from 1-6 in the `site/config.php`. The function, the shortcut (meta+1, meta+2, ...) as well as the icon number will adjust accordingly.

Example:
````
c::set('textarea.h1', 'h2');
c::set('textarea.h2', 'h3');
c::set('textarea.h3', 'h4');
````

### Buttons

You can globally define what the default buttons should be. By default all buttons are displayed. If you don't need the `h1` and `email` buttons for example, put the following in your `config.php`:

````
c::set('textarea.buttons', array(
  "h2",
  "h3",
  "bold",
  "italic",
  "ulist",
  "olist",
  "link",
  "page"
));
````


If you want to override this for a single field just use `buttons:` as you would with the built-in textarea:

````
test:
  type: textarea
  buttons:
    - h1
    - h2
    - bold
    - olist
    - link
````
