# How to build on x86\_64 Linux distribution #

In order to build under x64 distribution there should be several packages installed. In my case it is Kubuntu 10.04 x86\_64, for other distributions it may differ.

# 0. Follow install procedure from x86 build environment: JetDroidBuildEnvironment

# 1. Libraries for x32 compatibility:

<pre>sudo apt-get install ia32-libs</pre>

# 2. Android specific libs:

<pre>sudo apt-get install g++-multilib</pre>

<pre>sudo apt-get install lib32z1-dev</pre>

<pre>sudo apt-get install lib32ncurses5-dev</pre>
