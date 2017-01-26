ip_to_asn
=========
Resolve IPs to their ASNs and display total IPs per ASN.  


Usage
-----
```
usage: ip_to_asn FILE
Resolve IPs to their ASNs and display total IPs per ASN.

REQUIREMENTS:
  - GNU netcat
  - Python 3.x

ARGUMENTS:
This sends FILE as a bulk query to Team Cymru’s WHOIS database. (See the
documentation at http://www.team-cymru.org/IP-ASN-mapping.html#whois for
file-format details.)

Example file:

begin
verbose
8.8.8.8
68.22.187.5
end

SOURCE:
https://github.com/princebot/ip_to_asn
```


TODO
----
* Complete README.
* Try out [bats](https://github.com/sstephenson/bats) for unit testing.
* Sort results by IP address after initial sort by ASN.
* Test with large list (50K+) of IPs for input.
* Add (more easily) machine-parsable output.
* Check time effort/cost of implementing this as a `pip`-installable Python
  program instead (less black magic, simpler to install and test).
* … But don’t get carried away, because you have other stuff to do.
  :stuck_out_tongue:
