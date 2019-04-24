# zOS-files
My standard configuration files for setting up services on z/OS (such as Communications Server).

## Why?
I find myself often having to create a new configuration on a new system, or consulting on how to set up something on z/CS (usually OSPF or Policy Agent these days). Rather than creating from scratch (using increasingly rusty memory) or from pages on the Net, it seemed like a good idea to put them somewhere accessible.

Inspired by https://github.com/davewongillies/dot-files :)

Once everyone changes over to using the Configuration Assistant under z/OSMF though, this will possibly become obsolete though!

## Content
TCP/IP examples include:
* TCPIP.PROFILE (with the port reservations I usually run)
  * two versions -- monolithic and INCLUDE-based
* OMPROUTE.CONF to correspond
* SNMPD configuration files
* Policy Agent configuration
  * sample TN3270 and FTPS configurations

Supporting configuration files such as ENVVARS and others will be included also.

SNA Services
Examples include my start list (my common VTAMOPTS), as well as major nodes for the following:
* XCA for Enterprise Extender (MEDIUM=HPRIP)
* Switched PU definitions for DLUR-supported PUT2)
* Switched PU definitions for PUT2.1 (for those that don't want DYNPU=YES)
* possibly others
