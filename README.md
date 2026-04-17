fedora-active-user
==================

[![Build Status](https://travis-ci.org/pypingou/fedora-active-user.svg?branch=master)](https://travis-ci.org/pypingou/fedora-active-user)

This script generates a small report of the recent activity
of a fellow Fedora contributor using either their FAS (Fedora
Account System) login (recommended) or their email address.

The script checks:

- last builds on koji
- last update on Bodhi
- last update on Bugzilla (takes a while)
- last email set to mailing lists
- last actions recorded by fedmsg
The mailing lists considered are set at the top of the script, at
the moment, they are:
  fedora.devel
  fedora.artwork
  fedora.desktop
  fedora.epel.devel
  fedora.extras.packaging
  fedora.fonts
  fedora.general
  fedora.infrastructure
  fedora.kde
  fedora.perl
They are checked using gmane's function to search by sender's email.

This script depends on the [fedora-cert package](https://pagure.io/fedora-packager).
