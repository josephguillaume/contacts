# contacts

Address book-like application to manage contact information. 

Forked from https://github.com/linkeddata/contacts to use `solid-auth-fetcher` and `contacts-pane` compatible schema.

Addressbooks (`VCARD:AddressBook`) are stored in a `pim:Workspace`, linked from a `pim:PreferencesWorkspace` (e.g. `/Applications/`) specified in the user's `pim:preferencesFile`. Contacts are loaded by looking for a `VCARD:groupindex` and its `VCARD:group`(s).

Note that contacts from the previous version will not be loaded without a new `VCARD:groupindex` and `VCARD:group` (they were previously loaded by globbing from the `VCARD:AddressBook`).


Quick Start for contributors
----------------------------

```
$ git clone git://github.com/josephguillaume/contacts
$ cd contacts
$ sudo npm -g install bower
$ bower install
```
