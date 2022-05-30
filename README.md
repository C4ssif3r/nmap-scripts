nmap-vulners-nse scripts

# USAGE:

 nmap -sV --script vulners.nse [--script-args mincvss=<arg_val>] <target>
  
  ex1:
           nmap -sV --script vulners.nse --script-args mincvss=5.0 <target>
  
args vulners.mincvss Limit CVEs shown to those with this CVSS score or greater.
----------------------
# output

53/tcp   open     domain             ISC BIND DNS
-- | vulners:
-- |   ISC BIND DNS:
-- |     CVE-2012-1667    8.5    https://vulners.com/cve/CVE-2012-1667
-- |     CVE-2002-0651    7.5    https://vulners.com/cve/CVE-2002-0651
-- |     CVE-2002-0029    7.5    https://vulners.com/cve/CVE-2002-0029
-- |     CVE-2015-5986    7.1    https://vulners.com/cve/CVE-2015-5986
-- |     CVE-2010-3615    5.0    https://vulners.com/cve/CVE-2010-3615
-- |     CVE-2006-0987    5.0    https://vulners.com/cve/CVE-2006-0987
-- |_    CVE-2014-3214    5.0    https://vulners.com/cve/CVE-2014-3214
 
  
--------------------
# screen shot for vulners.nse:
  ![example](https://user-images.githubusercontent.com/79422726/170949276-1a3d7f8c-33aa-46f2-a2fc-7fd10c3c6e64.png)

  
  
  # patch rejex patch examples:
      ![paths_regex_example](https://user-images.githubusercontent.com/79422726/170950117-69dbf6b9-a4c8-46f7-888a-babf6c982162.png)

  
  # simple rejex patch example:
      ![simple_regex_example](https://user-images.githubusercontent.com/79422726/170950530-65e60d4a-6f44-4352-8854-d6ee3f684f25.png)
