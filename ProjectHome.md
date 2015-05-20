

## News ##

# **Plecost in Pentoo http://se-united.org/plecost-in-pentoo/**

# **Now we use Wingware Python IDE!**

[Wingware](http://wingware.com/)
<img src='http://wingware.com/images/coded-with-logo-129x66.png' />

# **[BackTrack 5](http://www.backtrack-linux.org/) also includes Plecost. Our fish is already in three fishbowl (BackBox, Blackbuntu and BackTrack). Great!**

# **[Blackbuntu](http://www.blackbuntu.com/) also includes Plecost. Thanks for the trusted.**

# **Plecost "0.2.2-9-beta" added in [BackBox](http://www.backbox.org). You can read a review in [iniqua.com](http://www.iniqua.com/2010/12/25/backbox-linux/)**

# **New release 0.2.2-9-beta available: Fixed plugin list reload problem.**

  * _Wordpress.com has changed plugin list. Therefore the option -R
(Reload plugin list) doesn't work properly. Please be patient, the problem
will be solved soon._

# **Also includes a new verification:** Now you can see the latest version
of wordpress released after the version found.

`==> Results for: http://blogs------- <==`

`[i] Wordpress version found:  2.6.1`

`[i] Wordpress last public version: 3.0.1`


## General description ##

_Wordpress finger printer tool_, plecost search and retrieve information
about the plugins versions installed in Wordpress systems. It can analyze
a single URL or perform an analysis based on the results indexed by Google.
Additionally displays CVE code associated with each plugin, if there.

Plecost retrieves the information contained on Web sites supported by
Wordpress, and also allows a search on the results indexed by Google.

## Site ##

http://www.iniqua.com/labs/

## Libraries ##

[xgoogle](http://www.catonmat.net/blog/python-library-for-google-search/)

## Quick help ##

Plecost works in two modes. On the one hand by analyzing a single URL
and the other analyzing the results of Google searches (-G).

### Threads version ###

```
Usage: ./plecost-0.2.2-8-beta.py [options] [ URL | [-l num] -G]

Google search options:
    -l num    : Limit number of results for each plugin in google.
    -G        : Google search mode
    
Options:
    -n        : Number of plugins to use (Default all - more than 7000).
    -c        : Check plugins only with CVE associated.
    -R file   : Reload plugin list. Use -n option to control the size
    -o file   : Output file. (Default "output.txt")
    -i file   : Input plugin list. (Need to start the program)
    -s time   : Min sleep time between two probes. Time in seconds. (10)
    -M time   : Max sleep time between two probes. Time in seconds. (20)
    -t num    : Number of threads. (Default 1)
    -h        : Display help. (More info: http://iniqua.com/labs/) 

Examples:

  * Reload first 5 plugins list:
        plecost -R plugins.txt -n 5
  * Search vulnerable sites for first 5 plugins:
        plecost -n 5 -G -i plugins.txt
  * Search plugins with 20 threads, sleep time between 12 and 30 seconds for www.example.com:
        plecost -i plugin_list.txt -s 12 -M 30 -t 20 -o results.txt www.example.com    
```

<img src='http://www.iniqua.com/wp-content/uploads/2010/03/plecost-0.2.2-8-beta.png' />


### Mono task version ###

```
Usage: ./plecost_0.0.1-5beta.py [options] URL | [options] -G

Options:
-G      : Google search mode
-n      : Number of plugins to use (Default all - more than 7000).
-c      : Check plugins only with CVE associated.
-R file : Reload plugin list. Use -n option to control the extension 
-o file : Output file. (Default "output.txt")
-i file : Input plugin list. (Need to start the program)
-s time : Min sleep time between two probes. Time in seconds. (Default 10)
-M time : Max sleep time between two probes. Time in seconds. (Default 20)
-h      : Display help. (More info: http://iniqua.com/labs/)

Examples:

* Reload first 5 plugins list:
     plecost -R plugins.txt -n 5
* Search vulnerable sites for first 5 plugins:
     plecost -n 5 -G -i plugins.txt
* Search plugins with sleep time between 12 and 30 seconds for www.example.com:
     plecost -i plugin_list.txt -s 12 -M 30  -o results.txt www.example.com 
```

<img src='http://www.iniqua.com/wp-content/uploads/2010/03/output_plecost.png' />


## Changelog ##

**0.2.2-9-beta:**

  * Fixed Wordpress plugin list load.
  * Added current Wordpress version.


**0.2.2-8-beta & 0.2.2-7-beta**

  * Fixed some execition errors.

**0.1-6-rt-beta**

  * Threads support added.

**0.0.1-4beta**

  * Improved Google search.
  * Cast errors.

**0.0.1-2beta**

  * Raise exception when URL opened not exits.
  * Raise exception when plugins list file is not accesible.
  * Restructured form that command line input parameters was collected.
  * Changed serveral graphi

**0.0.1-1beta**

  * Added compatibility with spanish readme.html

**0.0.1beta**

  * First release

## In the Web ##

http://www.securitybydefault.com/2010/03/seguridad-en-wordpress.html

http://www.securitybydefault.com/2011/11/identificacion-de-vulnerabilidades-en.html

http://www.clshack.it/plecost-a-wordpress-penetration-test-for-plugins

http://securityetalii.wordpress.com/2010/03/06/auditando-wordpress-con-plecost/

http://loginroot.diosdelared.com/?coment=6116

http://ayudawordpress.com/securidad-en-wordpress/

http://www.ehacking.net/2012/05/wordpress-security-vulnerability.html

