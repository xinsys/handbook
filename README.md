18F Handbook [![Build Status](https://travis-ci.org/18F/handbook.svg?branch=master)](https://travis-ci.org/18F/handbook)
========================

The [18F Handbook](https://handbook.18f.gov) documents the mission, values, structures, policies, tools, and guides that shape our team. This is a _living_ document and is updated regularly. If you have questions, comments, or suggestions, please
[open an issue](https://github.com/18F/handbook/issues). If you want to add content to the Handbook, please submit a pull request or ask in [#18f-handbook](https://18f.slack.com/messages/18f-handbook).

Note: If you're changing any kind of process, please let [#wg-onboarding](https://18f.slack.com/messages/wg-onboarding) know so we can keep the handbook, new hire messages, and checklists up to date.

# Development

``` bash
git clone https://github.com/18F/handbook.git
cd handbook
bundle install
./go serve
```

## Travel guide development
To add additional images:
* Add an image to the `images/travel` directory
* Link the image on the travel page, with folding HTML: `<img src="/images/travel/filename.png" class="travel-guide-hide">`
* A show/hide link will automatically be created.

To create a new page:
* Create a markdown file in the `_pages/policies/travel` directory
* Include a title and links to the "Travel Guide TOC" (see existing pages for reference)
* Update the page content
* Update the Travel Guide TOC `_pages/policies/travel/travel-guide-table-of-contents.md` with a link to your new page.
