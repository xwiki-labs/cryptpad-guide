# Setting up a CryptPad instance

## Disclaimer

The CryptPad project employs three full-time engineers.
Collectively, we are responsible for:

* oversight of the project's online spaces (GitHub, Riot, IRC)
* UI/UX design of the platform in response to user's needs
* regular security audits to ensure that data trusted to the platform remains safe
* ongoing maintenance and the continued development of new features
* manual and automated testing for quality assurance
* documentation of the project so that the software is accessible to anyone who wants to use it
* the administration of CryptPad.fr
* support for the paying subscribers that contribute to the project's financial sustainability
* promotion of the project, both online and in person at a variety of events
* grantwriting to ensure that we can continue to advance the project

We are very committed to our work and to ensuring that anyone can use our software, however, there is only so much time in any given day and we must prioritize the actions that we believe will have the most positive overall impact.

Our policy is to explicitly support the configurations which we use ourselves.
While we make a best effort to support other use-cases we can't possibly support them all with our current resources.
Consequently, we assume no responsibility for any installation guides or recommended practices by any individual or organization not explicitly recommended within this official documentation.

## Supporting development

There are a number of ways in which you can help to support the project.
If your time is limited you can help through by making a one-time or monthly donation to [our OpenCollective campaign](https://opencollective.com/cryptpad).
Otherwise if you want to contribute your services to the project, we suggest that you join [our community chat room](https://riot.im/app/#/room/#cryptpad:matrix.org) and let us know how you're interested in helping.
While you don't need our permission to use or modify any of our code, chatting with us or our community first can help to maximize our collective effort and ensure that you don't start working on something that is already in progress.

You don't need to be able to write code in order to get involved.
We struggle to keep our documentation up-to-date, so if you discover anything that you think might be incorrect or incomplete you are welcome to propose a correction.
CryptPad is only partially translated in most of its supported languages, so you may be in a position to contribute through our [translation platform](https://weblate.cryptpad.fr/projects/cryptpad/app/).

We have a very small budget for promoting ourselves and welcome any effort help to spread the word about the project.
Sharing a link to a CryptPad instance along with your honest experience with it through Twitter, the Fediverse, Reddit, or any other social media can expose thousands of people to the platform with a single click.
Likewise, using the platform collaboratively with your peers in place of an unencrypted alternative helps a lot, as the project's value is most apparent when used socially.
If you're interested in speaking about the project in a public venue we may be able to help offer advice, content, or promotional materials to help make it happen.

Finally, we plan to share our long-term roadmap publicly.
If you are able to modify and improve the platform's code and you see any features that aren't currently under development, we welcome pull requests.
CryptPad is an unconventional platform and our roadmap will not always be complete, so again, chatting with us before investing a lot of time may help save you some effort.

## Supported configurations

We explicitly support the use of CryptPad in two main configurations:

1. a standalone JavaScript server intended for use as a development platform
  * installed on a modern Linux distribution using [nvm](https://github.com/nvm-sh/nvm)
2. a production-grade installation based on the project's flagship instance ([CryptPad.fr](https://cryptpad.fr))
  * using Debian9, nginx, node v12.14.0, with source managed using git, npm, and bower

Other operating systems (Windows, BSD), webservers (Apache, Traefik), or deployment methods (compressed archives, containers) may work with trivial modifications, however, we neither test them nor use them ourselves.
Any questions or issues regarding alternate configurations should be directed to the authors of whatever installation guide suggested their use.
To be clear this is not a statement about the quality of any other software, we merely cannot afford to support every possible use-case with our current budget.


* What you'll need for a production installation
  * root access to a linux-based host
  * administrative rights for a DNS address
  * an email address that you're comfortable sharing with your users
  * a modern web browser for testing your configuration




* XXX WIP
* Common issues
  * caching
    * static content
      * use incognito/private mode
    * CSP headers
  * incorrect CSP
* Recommended configuration
  * loginSalt
  * adminKeys
  * accounts and subscription button
  * adminEmail
  * customize/translations/message.js#Messages.home_host
  * supportMailbox
  * application_config#fileHost
* Additional measures
  * ./scripts/evict-inactive.js
  * backup
  * Certificate renewal
* Updating
  * getting notified of new releases
    * Twitter
    * Mastodon
    * IRC/Matrix
    * https://github.com/xwiki-labs/cryptpad/releases.atom
