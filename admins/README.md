# Setting up a CryptPad instance

* Disclaimer
  * three-person team
  * we support what we use
  * no liability
* Supporting development
  * WTFM
  * OpenCollective
  * Promoting the project
    * Reddit
    * Mastodon/Fediverse
    * Twitter
    * With friends/colleagues
* Supported configurations
  1. standalone Nodejs server for development
  2. nginx reverse proxy for production hosting
    * What you'll need for a production installation
      * root access to a linux-based host
      * administrative rights for a DNS address
      * an email address that you're comfortable sharing with your users
      * a modern web browser for testing your configuration
* Other configurations
  * Docker or other containers
  * Apache
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
  * appliction_config#fileHost
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
