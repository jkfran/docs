**Usage:** `juju show-offer [options] [<controller>:]<offer url>`

**Summary:**

Shows extended information about the offered application.

**Options:**

`-B, --no-browser-login (= false)`

Do not use web browser for authentication

`-c, --controller (= "")`

Controller to operate in

`--format (= tabular)`

Specify output format (`json|tabular|yaml`)

`-o, --output (= "")`

Specify an output file

**Details:**

This command is intended to enable users to learn more about the application offered from a particular URL. In addition to the URL of the offer, extra information is provided from the readme file of the charm being offered.

**Examples:**

To show the extended information for the application 'prod' offered from the model 'default' on the same Juju controller:

`    juju show-offer default.prod`

The supplied URL can also include a username where offers require them. This will be given as part of the URL retrieved from the `juju find-offers` command. To show information for the application 'prod' from the model 'default' from the user 'admin':

`   juju show-offer admin/default.prod`

To show the information regarding the application 'prod' offered from the model 'default' on an accessible controller named 'controller':

`   juju show-offer controller:default.prod`

**See also:**

[find-offers](https://discourse.jujucharms.com/t/command-find-offers/1722)
