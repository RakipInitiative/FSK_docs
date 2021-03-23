---
title: Installation of PMM-Lab
summary: Installation instructions of PMM-Lab
keywords: installation instructions of PMM-Lab
sidebar: pmmlab_sidebar
permalink: pmmlab_installation_index.html
folder: pages/PMMLab
---
# Installing PMM-Lab
![](assets/pmmlab_installation.png)

1. Configure the software site as explained in <a href="#installing-plugins">Installing plugins</a>.
2. Check PMM-Nodes and click *Next*.

# Installing FSK-Lab
FSK-Lab is based on R 3.4, [https://r-project.org](https://r-project.org), which is an essential component for it to function. FSK-Lab is supported on Windows, Mac and Ubuntu.

<div class="col-lg-12">
  <ul id="myTab" class="nav nav-tabs nav-justified">
    <li class="active"><a href="#fsk-windows" data-toggle="tab"><i class="fa fa-tree"></i>Windows</a></li>
    <li class=""><a href="#fsk-mac" data-toggle="tab"><i class="fa fa-car"></i>Mac</a></li>
    <li class=""><a href="#fsk-ubuntu" data-toggle="tab"><i class="fa fa-support"></i>Ubuntu</a></li>
  </ul>

  <div id="myTabContent" class="tab-content">
    <div class="tab-pane fade active in" id="fsk-windows">
      <h4>Installing R with bundles</h4>
      <p>For convenience some bundles with preconfigured R are included in the software site. You can pick either the 32 or 64 bit version depending of your operating system. If you already have R installed on your system and you prefere to use that version, do not check either of the options. The bundles are named:
        <ul>
          <li>R 3.4.4 for 64-bit Windows</li>
          <li>R 3.4.4 for 32-bit Windows</li>
        </ul>
      </p>
      <h4>Installing R manually</h4>
      <p>If R is already installed it can be configured to be used in FSK-Lab. First two R packages need to be installed. These can be easily installed in an R console with the command: <code>install.packages(c('Rserve', 'miniCRAN','svglite'))</code>.
      </p>
      <p>The path to R needs to be set in Preferences, FSK-Lab settings.
      <img src="assets/fsk_preferences.png" alt="FSK settings">
      </p>
    </div>
    <div class="tab-pane fade" id="fsk-mac">
      <p>On Mac it is necessary to install R 3.4.x from <a href="https://cran.r-project.org/bin/macosx/el-capitan/base/">https://cran.r-project.org/bin/macosx/el-capitan/base/</a>. FSK-Lab on Mac requires three packages: Rserve, miniCRAN and Cairo. These may be installed in the R console with: <code>install.packages(c('Rserve', 'miniCRAN', 'Cairo'))</code>. Besides these three packages, MacOS also requires the XQuartz software which can be obtained at <a href="http://xquartz.macos-forge.org">http://xquartz.macos-forge.org</a>.
      </p>
      <p>
        The path to the R folder to be entered in KNIME (as described for Windows) should be /Library/Frameworks/R.framework/Resources/.
        <img src="assets/fsk_preferences.png" alt="FSK settings">
      </p>
    </div>
    <div class="tab-pane fade" id="fsk-ubuntu">
      <p>
        First, Ubuntu requires some development libraries for the R packages that can be installed with apt-get in the terminal:
        <code>sudo apt-get install libcurl4-openssl-dev libssl-dev libxml2-dev</code>
      </p>
      <p>
        On Mac it is necessary to install the packages Rserve and miniCRAN that can be installed in the R terminal with:
        <code>install.packages(c('Rserve', 'miniCRAN'))</code>.
      </p>
      <p>
        The path to the R folder to be entered in KNIME should be: /usr/lib/R.
      </p>
    </div>
  </div>
</div>
