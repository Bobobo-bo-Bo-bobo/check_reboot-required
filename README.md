**_Note:_** Because I'm running my own servers for serveral years, main development is done at at https://git.ypbind.de/cgit/check_reboot-required/

----

Nagios check to determine if reboot is required
===============================================

## Preface

Not only a kernel upgrade but other packages as well require a system reboot, e.g. `dbus` or `glibc`.

This [Nagios](https://www.nagios.org/) check if a system reboot is required.

---

## Supported distributions

At the moment the following distributions distributions are supported

  * Debian 8 or newer
  * Redhat Enterprise Linux / CentOS 7 or newer

---

## Required packages
For all distributions `lsb_release` is required to determine the distribution and it's release version.

### Debian
Debian required the `reboot-notifier` package.

### Redhat Enterprise Linux / CentOS
`yum-utils` is required for CentOS / Redhat Enterprise Linux.

---

## Command line parameters

Supported command line parameters are:

  * `-h` or `--help` - shows a brief help
  * `-w` or `--warn` - only report warning instead of critical condition when a restart is required

---

## License
This program is licenses under [GLPv3](http://www.gnu.org/copyleft/gpl.html).

