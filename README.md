# Jekyll-Nows

Jekyll-Nows is a plugin that facilitates publishing a single-page personal bio site with an archive of updates using the not-yet-stable `collections` feature of Jekyll.

## Setup

Copy the `jekyll-nows.rb` file to the `_plugins` directory of your project.

Copy the `_layouts/now.html` and `_layouts/nows_index.html` files to the `_layouts` directory of your project.

Edit your `_config.yml` file to include the following lines:

```
collections:
  - nows
```

Create a `_nows` directory in the root directory of your project.

## Usage

Jekyll-Nows takes Markdown-formatted entries organized by date and formats them in its opinionated chronological archive style. These entries will be stored in the `_nows` directory. It is suggested that they have filenames in the format of `YYYY-mm-dd.md`, but any filenames will work.

Each ‘now’ entry has YAML topmatter with a single `date` element:

```
---
date: 2015-03-28
---

# Example

Here is an [example](http://example.com) entry.
```

## Plans

I use this plugin to generate my own [personal site](http://brianjon.es) and will continue to share improvements. My plan is to keep things simple and straightforward, but one planned expansion is to be able to display diffs between adjacent updates.

## ‘Nows’ in Use

I’d be very interested to hear about instances of using this style of biography archiving in the wild.

## License

The MIT License (MIT)

Copyright (c) 2015 Brian Jones

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.