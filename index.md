---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "2022 UC Carpentries Fall Workshop"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "Zoom"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "us"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the
latitude: "45"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-1"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "Sept. 6-13, 2022"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")

humantime: "9:00 am - 12:00 pm"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2022-09-06      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2022-09-13        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Scott Peterson (UCB)", "Reid Otsuji (UCSD)", "Kat Koziar (UCR)","Kimberly Thomas (UCSD)", "Zhiyuan Yao (UCLA)", "Christine Wells (UCLA)", "Scott Gruber (UCLA)", "Derek Devnich (UC Merced)", "Erin Foster (UC Berkeley)", "Kenji Hayashi (UCLA)", "Ryan Gan (El Camino)" ] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["Stephanie Labou (UCSD)", "Reid Otsuji (UCSD)", "Kristi Liu (UCSB)", "Kat Koziar (UCR)", "Kimberly Thomas (UCSD)", "Lisa Ngo (UCB)", "Leigh Phan (UCLA)", "Eastern Kang (UCSD)"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
contact: ["kkt008@ucsd.edu", "zyao@ucla.edu"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["timdennis@ucla.edu", "rotsuji@ucsd.edu", "speterso@library.berkeley.edu"]
collaborative_notes: https://codimd.carpentries.org/fwkQLM2ZTuCRirtE16WjBQ  # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
eventbrite:        # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)
---

<!--
  HEADER (above)
  Edit the values in the block above to be appropriate for your workshop.
  If the value is not 'true', 'false', 'null', or a number, please use
  double quotation marks around the value, unless specified otherwise.
  And run 'tools/check' *before* committing to make sure that changes are good.
-->

<!--
  EVENTBRITE
  This block includes the Eventbrite registration widget if
  'eventbrite' has been set in the header.  You can delete it if you
  are not using Eventbrite, or leave it in, since it will not be
  displayed if the 'eventbrite' field in the header is not set.
-->
{% if page.eventbrite %}
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="248px"
  scrolling="auto">
</iframe>
{% endif %}

<h2 id="general">General Information</h2>

<!--
  INTRODUCTION
  Edit the general explanatory paragraph below if you want to change
  the pitch.
-->
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
  This workshop is open to UCSD students, staff, and faculty.
</p>
<p>
  <strong>You don't need to have any previous knowledge of programming or the tools presented in the workshop to attend.  A laptop is required for each session.</strong>
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
  <strong>Requirements:</strong> Participants must bring a laptop with
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
  Please email kkt008@ucsd.edu or zyao@ucla.edu for more information.
</p>

<p id="certificate">
<strong>For UCSD students</strong>:
  A Co-Curricular of Record activity recognition may be requested for UCSD students who attend Day 1-3 plus one additional session day. 
  For more information on the UC San Diego Co-Curricular of Record (CCR), please visit the <a href="https://elt.ucsd.edu/ccr/index.html">UCSD Engaged 
  Learning Tools Co-Curricular Record page</a>.
</p>
<hr/>

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

/>
> 

-->
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
     <thead><tr> <th><strong>Date</strong></th> <th><strong>Session</strong></th> <th><strong>Topics</strong></th> </tr></thead>
     <tbody>
      <tr><td>Sept 6</td><td>Introduction to R - Part 1 <br> Introduction to Python - Part 1</td><td>Intro to R & RStudio - basics, data structures, and data import/export <br> Python: Running/Wuitting, Variables and Assignment, Data Types/Type Conversions, Built-in Functions, and Help</td></tr>
      <tr><td>Sept 7</td><td>Introduction to R - Part 2 <br> Introduction to Python - Part 2</td><td> R: dplyr and tidyverse <br> Python: Libraries, Writing Functions, Reading/Writing data in Dataframes, and Pandas Dataframes</td></tr>
      <tr><td>Sept 8</td><td>Introduction to R - Part 3 <br> Introduction to Python - Part 3</td><td> R: Plotting with ggplot2 and knitr <br> Python: Plotting, Lists, For Loops, Looping over Datasets, and Conditionals</td></tr>
      <tr><td>Sept 9</td><td> The Unix Shell</td><td> Introduction, Navigating the file system, & working with files & directories</td></tr>
      <tr><td>Sept 12</td><td> Version Control with Git</td><td> Introduction, Creating a Repository, Tracking Changes, and Collaborating</td></tr>
      <tr><td>Sept 13</td><td> SQL <br> OpenRefine </td><td> SQL:Introduction, Creating a Repository, Tracking Changes, and Collaborating <br> OpenRefine: OpenRefine: Cleaning and Transforming data</td></tr>
      </tbody></table>
  </div>
</div>

<h2 id="curriculum">Curriculum</h2>
<!-- R specific data information begins -->
<p id = "curriculum">
For this workshop we will be referencing the <a href="https://swcarpentry.github.io/r-novice-gapminder/">R for Reproducible Scientific Analysis</a>, <a href="http://swcarpentry.github.io/python-novice-gapminder/"> Plotting and Programming in Python</a>, <a href="https://librarycarpentry.org/lc-shell/">The UNIX Shell</a>, <a href="https://swcarpentry.github.io/git-novice/">Version Control with Git</a> , <a href="https://librarycarpentry.org/lc-sql/">SQL</a>, and <a href="https://librarycarpentry.org/lc-open-refine/">OpenRefine</a> Carpentries curricula. 
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
We will use HackMD collaborative notes for taking notes, and sharing URLs and bits of code. The links to each session are listed at this <a href="https://hackmd.io/Gb6tujHCR6ygyw9P37Xe5Q">link</a>.</p>

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

{% if site.carpentry == "swc" %}
{% include swc/setup.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/setup.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/setup.html %}
{% endif %}
