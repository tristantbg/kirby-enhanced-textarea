# Kirby Enhanced Textarea v1.1

![Preview](preview.png?raw=true)

## Installation

Download or clone this repository and put the "kirby-enhanced-textarea-master" folder into your `site/fields` folder and rename it to `textarea`. Alternatively you can also use the [Kirby CLI](https://github.com/getkirby/cli).

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

You don't need all the buttons? No problem, just use `buttons:` 

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
