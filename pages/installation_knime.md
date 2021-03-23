---
title: Installation instructions of KNIME
summary: Installation instructions of KNIME
keywords: installation
sidebar: fsklab_sidebar
permalink: installation_knime.html
folder: pages
---
KNIME must be installed.

# KNIME 3.7.2
KNIME 3.7.2 can be installed.

## Windows
| KNIME Analytics Platform version 3.7.2 for Windows | [64bit](http://download.knime.org/analytics-platform/win/KNIME%203.7.2%20Installer%20%2864bit%29.exe) |
| KNIME Analytics Platform version 3.7.2 for Windows | [32bit](http://download.knime.org/analytics-platform/win/knime_3.7.2.win32.win32.x86_64.exe) |

## Linux
| KNIME Analytics Platform version 3.7.2 for Linux | [64bit](http://download.knime.org/analytics-platform/linux/knime_3.7.2.linux.gtk.x86_64.tar.gz) |

## Mac OS X
| KNIME Analytics Platform version 3.7.2 for Mac OS X	| [64bit](http://download.knime.org/analytics-platform/macosx/knime_3.7.2.app.macosx.cocoa.x86_64.dmg) |

* Help with KNIME installation [https://www.knime.com/installation](https://www.knime.com/installation)


## Installing plugins
The FSK-Lab and PMM-Lab plugins are available at the KNIME update site:
[https://dl.bintray.com/silebat/fsklab_icpmf](https://dl.bintray.com/silebat/fsklab_icpmf).

<video width="706" height="700" controls="controls">
  <source src="assets/update_site.mp4" type="video/mp4">
</video>

Steps:

1. Download our Eclipse bookmarks from <a href="assets/fsk_bookmarks.xml" download>here</a>. This file contains the configuration to our KNIME update site.
2. Import this file from KNIME in Help, Install new Software and Manage.
3. In the *Available Software Sites* window click on *Import* and browse the file you downloaded in step 1. After importing successfully you should be back to the *Available Software Sites* and a new site called *FSK-Lab* should aoppear.
4. If you click *Apply and Close* you will return to the *Install* dialog you opened in step 1. Now you should be able to pick the *FSK-Lab* software site in the *Work with:* entry by clicking the blue arrow.
5. When the *FSK-Lab* software site is selected all the plugins published there including PMM-Lab and FSK-Lab are listed there. They can be checked and install by clicking on Next or Finish.

# Recommended optimization of KNIME
{% include warning.html title="Warning" content="A bad configuration can break KNIME and this is only recommended for expert users" %}

The configuration file *KNIME.ini* allows to optimize KNIME. To apply the changes KNIME must be started after saving the changes to this file.

1. The amount of RAM available in KNIME might be extended by changing the value of `-Xmx`. For example `-Xmx4g` indicates that 4GB RAM should be used.
2. If the connection to a KNIME server through KNIME fails, it might help to increase the response time. Simply add the line `-Dcom.knime.enterprise.client.connect-timeout=10000`.


# KNIME 4
Coming soon.
