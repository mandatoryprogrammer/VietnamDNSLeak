![Vietnam Flag](https://i.imgur.com/pslJoHb.png)

# Vietnam .vn TLD Zone Data

On Aug 31, 2017 at approximately 4:14AM PDT (earliest known detection), one of Vietnam's top level nameservers was accidentally configured to allow global DNS zone transfers. This allows anyone who performs an `AXFR` (zone transfer) request to the country's `f.dns-servers.vn` nameserver to get a copy of the nation's top level DNS data. This was detected by the [TLDR Project](https://github.com/mandatoryprogrammer/TLDR) - an effort to attempt zone transfers against all top level domain (TLD) nameservers every three hours and keep a running Github repo with the resulting data. The size of this leak is fairly big so this repository is meant to give a better overview of all the DNS data that is now available. It appears that previously these zone files have even been [sold for profit,](https://domains-index.com/downloads/vn-vietnam-current-domains-list-download-vn-zone-file/) so we are happy to give this data out to the public to enjoy/use in their research.

Note: As of the time of this writing Vietnam has again disabled zone transfers for its `f.dns-servers.vn` nameserver. This Github serves as a historical archive of the snapshot of Vietnam's DNS.

Special thanks to [Michel Gaschet](https://twitter.com/Michel_Gaschet) who (upon seeing the incident via TLDR) went and enumerated all of Vietnam's domain suffixes and compiled this dataset. All credit goes to him for enumerating all the various SLDs included in this repo!

[Click here for the commit showing this incident.](https://github.com/mandatoryprogrammer/TLDR/commit/5c7871c42f494cdc7c5e84f4c1c62f0c8a52dabb#diff-c66f3607b376ad44e60fcf513fb7a4f6)

### Number of Domain Names Leaked
* `.vn`: 947,222 entries.
* `.com.vn`: 358,877 entries.
* `.edu.vn`: 43,972 entries.
* `.net.vn`: 21,947 entries.
* `.name.vn`: 17,329 entries.
* `.org.vn`: 7,064 entries.
* `.gov.vn`: 4,108 entries.
* `others`: 2,898 entries. (All entries of others domains managed by ccTLD `f.dns-servers.vn` nameserver)
* `.info.vn`: 2,123 entries.
* `.pro.vn`: 1,257 entries.
* `.biz.vn`: 929 entries.
* `.ac.vn`: 308 entries.
* `.int.vn`: 59 entries.

Total entries: 1,408,093
