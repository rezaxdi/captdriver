# captdriver

## Foreword
Are you still using an older Canon laser printer that doesn't support
network printing, PCL or EPS? Does your printer only work with the
proprietary Canon Advanced Printing Technology (CAPT) driver software?
Did attempts at getting `ccpd` to work lead you nowhere? Or are you 
averse to the practice of installing 32-bit dependencies on a 64-bit
system?

**Captdriver is a free (as in speech) alternative driver** for Canon 
printers that can only accept the proprietary CAPT data stream format.
Captdriver allows the use of such printers in any operating system with 
a working copy of *CUPS*.

## Motivations
While *macOS* and *Microsoft Windows* users will have a generally 
satisfactory experience with those proprietary drivers, the same cannot
be said for many of us not running these operating systems.

Captdriver aims to provide an free and open-source alternative means
to using CAPT-only printers that can be maintained by the general public,
and thus be improved to provide a better user experience.

## Acknowledgements
This driver is an onging work in progress, based on the works of
Rildo Pragana, Nicholas Boichat, Alexey Galakhov, Benoit Bolsee as
well as Vitaliy Tomin.

This repository is merely a curated version of Galakhov's repository.
The code base will be kept identical for the time being; the only
difference is the presence of additional documentation.

## Status
The driver has been recently tested at time of writing to work with
a Canon Laser Shot LBP 3000. Success with the LBP 2900 has also been
reported. Reports on more devices are wanted and will be much appreciated.
@agalakhov has pretty much nailed it with the CAPT data stream format and
control routines, but more work is needed before captdriver can match the
experience in macOS and Windows.

The installation process is rather clumsy, but the driver is believed
to have a superior chance of enabling printers to work on some operating
systems such as GNU/Linux distributions (_Arch Linux_, _Alpine Linux_, 
_Debian_,  _Fedora_, _Ubuntu_,...).

Some annoyances remain, such as the need to restart printers after
**every** job to continue with the next, and generally inferior 
performance to that experienced in macOS and Windows.

## Installation and Setup
This software must be manually installed. Please review the 
`INSTALL.md` file for detailed instructions.

## Technical Information
Details of the CAPT format, including printer control
protocols, status registers and compression algorithms are
documented in the `SPECS` file. While incomplete and expected to
contain errors and omissions, help with expanding it and making
corrections is greatly appreciated. Please also check the 
[wiki] for more information.

## Disclaimers
Please use this driver at your own risk. As with any software licensed
under the *GNU General Public License 3.0*, there is NO WARRANTY.

This is unofficial software not endorsed by Canon Inc. or any of its
affiliates.

CUPS and macOS are trademarks of Apple Inc.

Windows is a trademark of Microsoft Corporation.

[ibm]: https://www-01.ibm.com/support/docview.wss?uid=nas8N1019527 "IBM. IBM Information on Printers by Canon. IBM Support. 
Reference #N1019527. Updated 2017-03-28."

[wiki]: https://github.com/mounaiban/captdriver/wiki "Mounaiban's captdriver Wiki."
