---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "2023 UC Carpentries Fall Workshop"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "Zoom"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "us"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the
latitude: "45"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-1"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "Sept. 11-21, 2023"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "8:30 am - 12:30 pm"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2023-09-11      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2023-09-21        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: [ "Scott Peterson", "Reid Otsuji", "Kim Thomas", "Albert Lee", "Echelle Burns", "Scott Peterson", "Geoffrey Boushey", "David Palmquist", "Lisa McAulay", "Jamie Jamison", Derek Devnich", "Saulo Soares" ] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: [ "Rosana Aguilera", "Celeste Allaband", "Jean Allen", "Kristian Allen", "Misha Coleman", "Stephanie Labou", "Devontae Baxter", "Monique Surles-Zeigler", "Ellen Davenport" ]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
contact: ["carpentries@ucsd.edu"]  # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["timdennis@ucla.edu", "rotsuji@ucsd.edu", "speterso@library.berkeley.edu"]
collaborative_notes: ["TBD"] # optional: URL for the workshop collaborative notes, e.g. an HackMD or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
---

<!--
  HEADER (above)
  Edit the values in the block above to be appropriate for your workshop.
  If the value is not 'true', 'false', 'null', or a number, please use
  double quotation marks around the value, unless specified otherwise.
  And run 'tools/check' *before* committing to make sure that changes are good.
-->

<!--
  INTRODUCTION
  Edit the general explanatory paragraph below if you want to change
  the pitch.
-->

<hr/>
<h2 id="general">General Information</h2>
<p>
  <a href="{{site.swc_site}}">The Carpentries</a>
  aims to help researchers get their work done in less time and with less pain by teaching them basic research computing skills. 
  This workshop is designed for researchers and enables non-experts to develop computing skills for research analysis. We will cover 
  basic concepts and tools, such as - working with libraries and data frames; reading and plotting data; creating and using functions; 
  the shell using command-line applications; cleaning and transforming data; and more. Participants will be encouraged to help one another 
  and to apply what they This is a free workshop and is open to all University of California students, staff, and faculty. 
  have learned to their own research problems.
</p>

<p>
  <em>
    For more information on what we teach and why,
    please see our paper
    "<a href="http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745">Best Practices for Scientific Computing</a>".
  </em>
</p>

<!--
  AUDIENCE
  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->
<p id="who">
  <strong>Who:</strong>
  This workshop is open to University of California students, staff, postdocs, and faculty. <strong>You don't need to have any previous knowledge of programming or the tools presented in the workshop to attend.  A laptop is required for each session.</strong>
</p>

<!--
  LOCATION
  This block displays the address and links to maps showing directions
  if the latitude and longitude of the workshop have been set.  You
  can use http://itouchmap.com/latlong.html to find the lat/long of an
  address.
-->
{% if page.latlng %}
<p id="where">
  <strong>Location:</strong>
  {{page.address}}.
</p>
{% endif %}

<!--
  SPECIAL REQUIREMENTS
  Modify the block below if there are any special requirements.
-->
<p id="requirements">
  <strong>Requirements:</strong> Participants must have a laptop or desktop with
  a few specific software packages installed (listed
  <a href="#setup">below</a>).
</p>

<!--
  CONTACT EMAIL ADDRESS
  Display the contact email address set in the header.  If an address
  isn't set in the header, the Software Carpentry admin address is
  used.
-->
<p id="contact">
  <strong>Contact</strong>:
  Please email carpentries@ucsd.edu for more information.
</p>
<!--
<p id="certificate">
<strong>For UCSD students</strong>:
  A Co-Curricular of Record activity recognition may be requested for UCSD students who attend Day 1-3 plus one additional session day. 
  For more information on the UC San Diego Co-Curricular of Record (CCR), please visit the <a href="https://elt.ucsd.edu/ccr/index.html">UCSD Engaged 
  Learning Tools Co-Curricular Record page</a>.
</p>
<hr/>
-->
<!-- Below is the official Carpentries Code of Conduct information -->

<h2 id="code-of-conduct">Code of Conduct</h2>

<p>
Everyone who participates in Carpentries activities is required to conform to the <a href="https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html">Code of Conduct</a>. This document also outlines how to report an incident if needed.
</p>

<p class="text-center">
  <a href="https://goo.gl/forms/KoUfO53Za3apOuOK2">
    <button type="button" class="btn btn-info">Report a Code of Conduct Incident</button>
  </a>
</p>

<hr/>

<!-- Below is the official Carpentries Survey links -->

<h2 id="surveys">Surveys</h2>
<p>Please be sure to complete these surveys before and after the workshop.</p>
<!--<p>pending<p>-->

<!-- to add survey go to 'layouts' folder >  'workshops.html' and update to "<meta name="slug" content="{{site.github.project_title}}"
then make sure the '_config.yaml' file has updated workshop_repo and workshop_site links -->

<p><a href="{{ site.swc_pre_survey }}{{ site.github.project_title }}">Pre-workshop Survey</a></p>
<p><a href="{{ site.swc_post_survey }}{{ site.github.project_title }}">Post-workshop Survey</a></p>

<hr/>

<!--
  SCHEDULE
  Show the workshop's schedule.  
-->
<h2 id="schedule">Schedule</h2>
<div class="row">
  <div>
    <table class="table">
     <thead><tr> <th><strong>Date</strong></th> <th><strong>Day</strong></th> <th><strong>Topics</strong></th> </tr> </thead>
     <tbody>
      <tr><td>Sept 11</td><td> Day 1 </td><td> The Unix Shell: Introduction, Navigating the file system, & working with files & directories</td></tr>
      <tr><td>Sept 12</td><td> Day 2 </td><td> Version Control with Git: Introduction, Creating a Repository, Tracking Changes, and Collaborating</td></tr>
      <tr><td>Sept 13</td><td> Day 3 </td><td> Intro to R & RStudio: basics, data structures, data import/export, dylyr </td></tr>
      <tr><td>Sept 14</td><td> Day 4 </td><td> Intro to R & RStudio: dplyr (cont.), tidyverse, plotting with ggplot2 and knitr </td></tr>
      <tr><td>Sept 18</td><td> Day 5 </td><td> Intro to Python: Running/writing, variables/assignment, data types/type conversions, built-in functions/help, libraries, reading/writing data in Dataframes, and Pandas Dataframes </td></tr>
      <tr><td>Sept 19</td><td> Day 6 </td><td> Intro to Python: plotting, lists, for loops, conditionals, looping over datasets, and writing functions </td></tr>
      <tr><td>Sept 20</td><td> Day 7 </td><td> Tidy Data: learn how to use this tool to clean, transform, and track changes made to data </td></tr>
      <tr><td>Sept 21</td><td> Day 8 </td><td> SQL:Introduction, Creating a Repository, Tracking Changes, and Collaborating </td></tr>
     </tbody></table>
  </div>
</div>
</hr>



<h2 id="curriculum">Curriculum</h2>
<!-- R specific data information begins -->
<p id = "curriculum">
For this workshop we will be referencing the <a href="https://swcarpentry.github.io/shell-novice/">The UNIX Shell</a>, <a href="https://swcarpentry.github.io/git-novice/">Version Control with Git</a>, <a href="https://swcarpentry.github.io/r-novice-gapminder/">R for Reproducible Scientific Analysis</a>, <a href="http://swcarpentry.github.io/python-novice-gapminder/"> Plotting and Programming in Python</a>, <a href="https://librarycarpentry.org/lc-spreadsheets/setup.html">Tidy Data</a>, and <a href="https://datacarpentry.org/sql-ecology-lesson/index.html">SQL</a> Carpentries curricula. 
</p>

<hr/>

<h2 id="datasect">Data</h2>
<!-- R specific data information begins -->
<p id = "data">
We will be using the specific software downloads and data for each lesson. Please refer to the listing of downloads needed for each session you'll be attending as provided at this <a href="https://hackmd.io/@U2NG/SJkaMk2t7">link</a>.</p>
<!-- R specific data information ends -->

<hr/>

<h2 id="collabnotes">Collaborative Notes</h2>
<!-- Python specific data information begins -->
<p id = "notes">
We will use HackMD collaborative notes for taking notes, and sharing URLs and bits of code. The links to each session are listed at this <a href="https://hackmd.io/vfJr8dEaQn-bKG2XoWZexw?edit">link</a>.</p>

<hr/>
<!--
  SETUP
  Delete irrelevant sections from the setup instructions.  Each
  section is inside a 'div' without any classes to make the beginning
  and end easier to find.
  This is the other place where people frequently make mistakes, so
  please preview your site before committing, and make sure to run
  'tools/check' as well.
-->

<h2 id="setup">Setup</h2>

<p>
  To participate in a
  {% if site.carpentry == "swc" %}
  Software Carpentry
  {% elsif site.carpentry == "dc" %}
  Data Carpentry
  {% elsif site.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  workshop,
  you will need access to the software described below.
  In addition, you will need an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>

{% comment %}
For online workshops, the section below provides:
- installation instructions for the Zoom client
- recommendations for setting up Learners' workspace so they can follow along
  the instructions and the videoconferencing

If you do not use Zoom for your online workshop, edit the file
`_includes/install_instructions/videoconferencing.html`
to include the relevant installation instrucctions.
{% endcomment %}
{% if online != "false" %}
{% include install_instructions/videoconferencing.html %}
{% endif %}

{% comment %}
These are the installation instructions for the tools used
during the workshop.
{% endcomment %}

<!-- Start of 'R' section. -->
<div id="r">
  <h3>R</h3>
  <p>
    <a href="https://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="https://www.rstudio.com/">RStudio</a>.
  </p>
  <div class="tab">
    <button class="tablinks" onclick="openTab(event,'RWindows')">Windows</button>
    <button class="tablinks" onclick="openTab(event,'RMacOS')">MacOS</button>
    <button class="tablinks" onclick="openTab(event,'RLinux')">Linux</button>
  </div>
  <div id="RWindows" class="tabcontent">
    <p>
      Install R by downloading and running
      <a href="https://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
      from <a href="https://cran.r-project.org/index.html">CRAN</a>.
      Also, please install the
      <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
      Note that if you have separate user and admin accounts, you should run the
      installers as administrator (right-click on .exe file and select "Run as
      administrator" instead of double-clicking). Otherwise problems may occur later,
      for example when installing R packages.
    </p>
    <p><strong>Video Tutorial:</strong> <a href="https://youtu.be/q0PjTAylwoU">SWC R Install Windows</a></p>
  </div>
  <div id="RMacOS" class="tabcontent">
    <p>
      Install R by downloading and running
      <a href="https://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
      from <a href="https://cran.r-project.org/index.html">CRAN</a>.
      Also, please install the
      <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
    </p>
    <p><strong>Video Tutorial:</strong> <a href="https://youtu.be/5-ly3kyxwEg">SWC R Install Mac</a></p>     
  </div>
  <div id="RLinux" class="tabcontent">
    <p>
      Instructions for R installation on various Linux platforms (debian,
      fedora, redhat, and ubuntu) can be found at
      <https://cran.r-project.org/bin/linux/>. These will instruct you to
      use your package manager (e.g. for Fedora run
      <code>sudo dnf install R</code> and for Debian/Ubuntu, add a ppa
      repository and then run <code>sudo apt-get install r-base</code>).
      Also, please install the
      <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
    </p>
  </div>
</div>

<!-- End of 'R' section. -->

<!-- Start of 'Python' section. -->
<div id="python">
  <h3>Python</h3>
  <p>
    We will teach Python using the <a href="https://jupyter.org/">Jupyter Notebook</a>,
    a programming environment that runs in a web browser (Jupyter Notebook will be installed by Anaconda). For this to work you will need a reasonably
    up-to-date browser. The current versions of the Chrome, Safari and
    Firefox browsers are all
    <a href="https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#browser-compatibility">supported</a>
    (some older browsers, including Internet Explorer version 9
    and below, are not).
  </p>
  <div class="tab">
    <button class="tablinks" onclick="openTab(event,'PythonWindows')">Windows</button>
    <button class="tablinks" onclick="openTab(event,'PythonMacOS')">MacOS</button>
    <button class="tablinks" onclick="openTab(event,'PythonLinux')">Linux</button>
  </div>
  <div id="PythonWindows" class="tabcontent">
    <ol>
      <li>Open <a href="https://www.anaconda.com/products/individual#download-section">https://www.anaconda.com/products/individual#download-section</a> with your web browser.</li>
      <li>Download the Anaconda for Windows installer with Python 3. (If you are not sure which version to choose, you probably want the 64-bit Graphical Installer <em>Anaconda3-...-Windows-x86_64.exe</em>)</li>
      <li>Install Python 3 by running the Anaconda Installer, using all of the defaults for installation <em>except</em> make sure to check <strong>Add Anaconda to my PATH environment variable</strong>.</li>
    </ol>
    <p><strong>Video Tutorial:</strong> <a href="https://youtu.be/xxQ0mzZ8UvA">SWC Install Python on Windows</a></p>
  </div>
  <div id="PythonMacOS" class="tabcontent">
    <ol>
      <li>Open <a href="https://www.anaconda.com/products/individual#download-section">https://www.anaconda.com/products/individual#download-section</a> with your web browser.</li>
      <li>Download the Anaconda Installer with Python 3 for macOS (you can either use the Graphical or the Command Line Installer).</li>
      <li>Install Python 3 by running the Anaconda Installer using all of the defaults for installation.</li>
    </ol>
    <p><strong>Video Tutorial:</strong> <a href="https://youtu.be/TcSAln46u9U">SWC Install Python on Mac</a></p>     
  </div>
  <div id="PythonLinux" class="tabcontent">
    <ol>
      <li>Open <a href="https://www.anaconda.com/products/individual#download-section">https://www.anaconda.com/products/individual#download-section</a> with your web browser.</li>
      <li>Download the Anaconda Installer with Python 3 for Linux.<br>
        (The installation requires using the shell. If you aren't
        comfortable doing the installation yourself
        stop here and request help at the workshop.)
      </li>
      <li>
        Open a terminal window and navigate to the directory where
        the executable is downloaded (e.g., `cd ~/Downloads`).
      </li>
      <li>
        Type <pre>bash Anaconda3-</pre> and then press
        <kbd>Tab</kbd> to autocomplete the full file name. The name of
        file you just downloaded should appear.
      </li>
      <li>
        Press <kbd>Enter</kbd>
        (or <kbd>Return</kbd> depending on your keyboard).
        You will follow the text-only prompts.
        To move through the text, press <kbd>Spacebar</kbd>.
        Type <code>yes</code> and press enter to approve the license.
        Press <kbd>Enter</kbd> (or <kbd>Return</kbd>)
        to approve the default location
        for the files.
        Type <code>yes</code> and press
        <kbd>Enter</kbd> (or <kbd>Return</kbd>)
        to prepend Anaconda to your <code>PATH</code>
        (this makes the Anaconda distribution the default Python).
      </li>
      <li>
        Close the terminal window.
      </li>
    </ol>
  </div>
</div>

<!-- End of 'Python' section. -->

<!-- Start of Unix Shell section. -->

<div id="shell">
  <h3>The Bash Shell</h3>
  <p>
    Bash is a commonly-used shell that gives you the power to do
    tasks more quickly.
  </p>
  <div class="tab">
    <button class="tablinks" onclick="openTab(event,'ShellWindows')">Windows</button>
    <button class="tablinks" onclick="openTab(event,'ShellMacOS')">MacOS</button>
    <button class="tablinks" onclick="openTab(event,'ShellLinux')">Linux</button>
  </div>
  <div id="ShellWindows" class="tabcontent">
    <ol>
       <li>Download the Git for Windows <a href="https://gitforwindows.org/">installer</a>.</li>
       <li>Run the installer and follow the steps below:
          <ol>
            <p>Git 2.27.0 Setup<p/>
            <li>Click on "Next" four times (two times if you've previously installed Git).  You don't need to change anything in the Information, location, components, and start menu screens.</li>
            <li><strong>From the dropdown menu select "Use the nano editor by default" and click on "Next".</strong></li>
              <p>Adjusting your PATH environment</p>
            <li>Ensure that "Git from the command line and also from 3rd-party software" is selected and click on "Next". (If you don't do this Git Bash will not work properly, requiring you to remove the Git Bash installation, re-run the installer and to select the "Git from the command line and also from 3rd-party software" option.)</li>
              <p>Choosing the SSH executable</p>
              <p>Choosing HTTPS transport backend</p>
            <li>Ensure that "Use the native Windows Secure Channel library" is selected and click on "Next".</li>
              <p>This should mean that people stuck behind corporate firewalls that do MITM attacks with their own root CA are still able to access remote git repos.</p>
              <p>Configuring the line ending conversions</p>
            <li>Ensure that "Checkout Windows-style, commit Unix-style line endings" is selected and click on "Next".</li>
              <p>Configuring the terminal emulator to use with Git Bash</p>
            <li><strong>Ensure that "Use Windows' default console window" is selected and click on "Next".</strong></li>
              <p>Configuring extra options</p>
            <li>Ensure that "Default (fast-forward or merge) is selected and click "Next"</li>
            <li>Ensure that "Enable file system caching" and "Enable Git Credential Manager" are selected and click on "Next".</li>
              <p>Configuring experimental options</p>
            <li>Click on "Install".</li>
              <p>Installing</p>
              <p>Completing the Git Setup Wizard</p>
              <p>as of 2020-06-02, the Window will say "click Finish", but the button is labelled as "Next"</p>
            <li>Click on "Finish" or "Next".</li>
          </ol>
      </li>
          <li>If your "HOME" environment variable is not set (or you don't know what this is):
            <ol>
              <li>Open command prompt (Open Start Menu then type <code>cmd</code> and press <kbd>Enter</kbd>)</li>
              <li>Type the following line into the command prompt window exactly as shown:
                <p><code>setx HOME "%USERPROFILE%"</code></p>
              </li>
              <li>Press <kbd>Enter</kbd>, you should see <code>SUCCESS: Specified value was saved.</code></li>
              <li>Quit command prompt by typing <code>exit</code> then pressing <kbd>Enter</kbd></li>
            </ol>
	  </li>
        </ol>
        <p>This will provide you with both Git and Bash in the Git Bash program.</p>
        <p><strong>Video Tutorial:</strong> <a href="https://www.youtube-nocookie.com/embed/339AEqk9c-8?modestbranding=1&playsinline=1&iv_load_policy=3&rel=0">Windows Installation</a></p>     
  </div>
  <div id="ShellMacOS" class="tabcontent">
    <p>The default shell in some versions of macOS is Bash, and Bash is available in all versions, so no need to install anything. You access Bash from the Terminal (found in <code>/Applications/Utilities</code>). See the Git installation <a href="#shell-macos-video-tutorial">video tutorial</a> for an example on how to open the Terminal. You may want to keep Terminal in your dock for this workshop.</p>
        <p>
            To see if your default shell is Bash type <code>echo $SHELL</code>
            in Terminal and press the <kbd>Return</kbd> key. If the message
            printed does not end with '/bash' then your default is something
            else and you can run Bash by typing <code>bash</code>
        </p>
        <p>
          If you want to change your default shell, see <a href="https://support.apple.com/en-au/HT208050" rel="noopener">
          this Apple Support article</a> and follow the instructions on "How to change your default shell".
        </p><strong>Video Tutorial</strong>
        <a href="https://www.youtube-nocookie.com/embed/9LQhwETCdwY?modestbranding=1&playsinline=1&iv_load_policy=3&rel=0">MacOS Installation</a>
   </div>
   <div id="ShellLinux" class="tabcontent">
      <p>
        The default shell is usually Bash and there is usually no need to
        install anything.
      </p>
      <p>
        To see if your default shell is Bash type <code>echo $SHELL</code> in
        a terminal and press the <kbd>Enter</kbd> key. If the message printed
        does not end with '/bash' then your default is something else and you
        can run Bash by typing <code>bash</code>.
      </p>
   </div>
</div>
<!-- End of Unix Shell section. -->

<!-- Start of Git section. -->
<div id="git">
  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported
    web browser</a>.
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already.
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
      for keeping your email address private</a> provided at GitHub.
  </p>
  <div class="tab">
    <button class="tablinks" onclick="openTab(event,'GitWindows')">Windows</button>
    <button class="tablinks" onclick="openTab(event,'GitMacOS')">MacOS</button>
    <button class="tablinks" onclick="openTab(event,'GitLinux')">Linux</button>
  </div>
    <div id="GitWindows" class="tabcontent">
      <p>
        Git should be installed on your computer as part of your Bash
        install (see the
        <a href="#shell">Shell installation instructions</a>).
      </p>
    </div>
    <div id="GitMacOS" class="tabcontent">
      <p>
        <strong>For macOS</strong>, install Git for Mac
        by downloading and running the most recent "mavericks" installer from
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
        Because this installer is not signed by the developer, you may have to
        right click (control click) on the .pkg file, click Open, and click
        Open on the pop up window.
        After installing Git, there will not be anything in your <code>/Applications</code> folder,
        as Git is a command line program.
        <strong>For older versions of OS X (10.5-10.8)</strong> use the
        most recent available installer labelled "snow-leopard"
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
      </p>
      <p><strong>Video Tutorial: </strong><a href="https://youtu.be/9LQhwETCdwY">SWC Install Shell, Git, and Nano on Mac</a></p>
    </div>
    <div id="GitLinux" class="tabcontent">
      <p>
      If Git is not already available on your machine you can try to
      install it via your distro's package manager. For Debian/Ubuntu run
      <code>sudo apt-get install git</code> and for Fedora run
      <code>sudo dnf install git</code>.
      </p>
    </div>
  </div>
</div>

<!-- End of Git section. -->


<!-- hiding SQL Lite insrtuctions -->
<div id="sql"> Start of 'SQLite' section.
  <h3>SQLite</h3>
  <p>
    SQL is a specialized programming language used with databases.  We
    use a simple database manager called
    <a href="http://www.sqlite.org/">SQLite</a> in our lessons.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="sql-windows">Windows</h4>
      <p>
        The <a href="{{site.swc_installer}}">Software Carpentry Windows Installer</a>
        installs SQLite for Windows.
        If you used the installer to configure nano, you don't need to run it again.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="sql-macosx">Mac OS X</h4>
      <p>
        SQLite comes pre-installed on Mac OS X.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="sql-linux">Linux</h4>
      <p>
        SQLite comes pre-installed on Linux.
      </p>
    </div>
  </div>

<!-- </div> End of 'SQLite' section. -->
<!--test note-->
<!--
{% if site.carpentry == "swc" %}
{% include swc/setup.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/setup.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/setup.html %}
{% endif %}
-->
