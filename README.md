18F Handbook [![Build Status](https://travis-ci.org/18F/handbook.svg?branch=master)](https://travis-ci.org/18F/handbook)
========================

The [18F Handbook](https://handbook.18f.gov) documents the mission, values, structures, policies, tools, and guides that shape our team. This is a _living_ document and is updated regularly. If you have questions, comments, or suggestions, please
[open an issue](https://github.com/18F/handbook/issues). If you want to add content to the Handbook, please submit a pull request or ask in [#18f-handbook](https://18f.slack.com/messages/18f-handbook).

Note: If you're changing any kind of process, please let [#wg-onboarding](https://18f.slack.com/messages/wg-onboarding) know so we can keep the handbook, new hire messages, and checklists up to date.

# What can't be included

For 18F staff, keep in mind that the handbook website and repository are public, so we can't include information that shouldn't be public. We already get training on this, but here are a few reminders about things we shouldn't include here:

* [Sensitive information, as described in our Open Source Policy practices guide](https://github.com/18F/open-source-policy/blob/master/practice.md#protecting-sensitive-information)
* Comments that can be easily interpreted as [endorsements](https://www.oge.gov/web/oge.nsf/Use%20of%20Government%20Position%20and%20Resources/17593AE8B3A597C685257E96006364E4?opendocument) (or other potential ethical issues)

We avoid including information that can easily go out of date and is already published somewhere else in a useful format. This includes: 

* People's phone numbers, even if public information (such as their GSA work number). Link to the public [GSA staff directory](http://www.gsa.gov/portal/staffDirectory/searchStaffDirectory) or the access-controlled 18F contact spreadsheet instead of including phone numbers in the handbook.
* Information that is already well-covered on GSA InSite. Link there instead of reproducing it.

We're careful about publishing [information collected during research](https://handbook.18f.gov/research-guidelines/); [learn more](https://docs.google.com/document/d/1Xp4LxbW6cx61rXrsnnfIPCz6cglovHzZeEjCcnpIeaM/edit) and ask [#research](https://18f.slack.com/archives/research) for guidance first.

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
