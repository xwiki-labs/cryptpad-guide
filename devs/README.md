# Working with CryptPad's code

* Assumptions
  * You have read the user and admin guides
  * You would like to read CryptPad's code to understand how it works
  * ...or you would like to modify CryptPad's code to change its behaviour
* Avoid duplicated effort
  * Talk to us
  * Review our roadmap
* Threat model
  * Publications
    * Private document editing with some trust
    * Behind the façade: paradigms of ubiquitous cryptography
* Subsystems
  * server
    * metadata
    * history keeper
    * rpc
    * blobs
    * activity/expiration
  * clients
    * worker
    * sandbox
    * pad encryption
    * login/registration
      * scrypt
    * mailbox encryption
    * chat encryption
    * teams
      * roster
    * passwords
    * CryptDrive
    * hashes
    * server-rpc


