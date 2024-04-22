# Changelog

## 9.0.0beta2

- Iplocation Extended Labels MMDB is added an option for MMDB download use cases.

## 9.0.0beta1

- Revamped the entire app for better performance and user experience.
- Added new flag 'restapi' and 'country_asn' for enhanced functionality.
- Included a new setup page to simplify initial configuration and settings.
- Introduced a new dashboard 'Overview' to provide a comprehensive summary of API and MMDB status.
- Implemented a new dashboard 'Log Status' section to monitor log activities more effectively.
- Added a new dashboard 'Force Refresh' for immediate MMDB updates.

## 8.9.1

- Iplocation Extended MMDB is added an option for MMDB download use cases.
- Iplocation Aggregated MMDB is added an option for MMDB download use cases.
- Privacy Extended MMDB is added an option for MMDB download use cases.

## 8.8.0

- Abuse MMDB is added an option for MMDB download use cases.
- Submit button during setup cannot be multi-clicked which previously caused simultaneous conflicting config-update requests to be fired.

## 8.7.0

- Fixed an issue where the setup page was not properly saving.
- Fixed an issue with warnings popping up when opening some UIs due to CSP issues.
- Removed unnecessary splunktalib code.

## 8.6.0

- Upgraded Splunk SDK version from 1.6.16 to 1.7.4.
- Stopped support for Splunk version 8.x.
- Fixed an issue where a default value for replicate_lookup was not provided in the custom app configuration files.
- Fixed an issue where the proxy type was incorrectly being propagated if entered as uppercase (e.g. 'HTTP') instead of lowercase (e.g. 'http'). This caused proxy setups to fail to properly make HTTP requests.
- Fixed an issue where MMDB files weren't being downloaded in distributed setups properly due to the way in which the API token was being retrieved in such a setup.
- Removed usage of replicationBlacklist and replicationWhitelist, which were deprecated in 9.x. Now use replicationAllowlist and replicationDenylist.

## 8.5.1

- Cloud compatibility fix was made.
- Fixed a bug where carrier data was not showing if company data is not available.
- Fixed a bug where on Windows machines the setup page produced a configuration file that was encoded as UTF-8-BOM, which the app was unable to open.
- Added support for standard_ip_hosted_domains.mmdb

## 8.4.0

- Support for streaming (only with mmdb)
- Other minor bug fixes.

## 8.3.1

- Performance Boost on MMDB Read
- Update on Default Dashboard
- Other minor bug fixes

## 8.2.0

- New Feature Option to Parallel download MMDB or Download once and sync later.
- Other minor bug fixes

## 8.1.0

- New Feature Manual Trigger to Sync the MMDB
- Fix IPV6 IP returning results on the Dashboard
- Disabled Replication to Indexing Layer
- Other Minor BugFixes

## 8.0.0

- Fix MMBD Bundle Accumulation Issues (old bundle gets deleted as new -MMDB bundle is downloaded)
- Fix ipinfo command to work in MMDB mode to work without "list_storage_password" capability.
- Other Minor BugFixes

## 7.1.1

- Persistent Setup Page
- Updated MMDB section on Setup Page
- Enhancement where MMDB is supported automatically on non-default management port.
- Other Minor BugFixes

## 7.0.8

- Bugfix multiple API calls or single IP lookup using ipinfo command
- Other Minor BugFixes

## 7.0.7

- NEW Setup Page for MMDB
- Support for all commands using MMDB and API
- Bugfix related to NULL values with ipinfo command
- Bugfix on issues with unauthenticated Proxy
- Other Minor BugFixes

## 6.0.1

- Updates to ipinfobatch command output
- New options available for ipinfo command
- Minor Bug fixes

## 5.7.4

- Bug Fixes with Authenticated Proxy
- Splunk Cloud Compatibility Package

## 5.7.3

- Support for Authenticated Proxy
- Splunk Cloud Compatibility Package

## 5.6.3

- Minor BugFixes with setup page

## 5.6.2

- Minor BugFixes with commands

## 5.6.1

- Adding a privacy=true flag so that the results are returned as part of the ipinfo command
- Support for multiple fields in one go , for example | ipinfo prefix=true src_ip, dest_ip

## 5.5.1

- Adding a privacy=true flag so that the results are returned as part of the ipinfo command and other Minor Bug Fixes

## 5.5.0

- Multi IP support with ipinfo command (eg |ipinfo src_ip dest_ip)

## 5.4.3

- Adding prefix=true support with ipinfo command

## 5.4.2

- Introducing lat/lon along with loc, for better support with maps

## 5.4.1

- Cleaning Up of Old Splunk Code and Minor Bug Fixes

## 5.4.0

- Support batching in privacy command

## 5.3.1

- Adding WorkFlow Action for IPinfo

## 5.2.10

- Updating Python Library to 1.6.15
- Bug Fixes with Batch Command

## 5.2.8

- Feature to Add custom rootCA certificate.
- Feature to Disable the SSL verification.
- Couple of other Bug fixes.

## 5.1.2

- Updating `ipinfo` command to support ipinfo bulk api

## 5.1.1

- Merging ipinfolookup capability with original ipinfo command
- privacyinfolookup to now be privacyinfo
- domaininfolookup to now be domaininfo
- rangesinfolookup to now be rangesinfo

## 5.0.2

- Support for Splunk Search Head Cluster

## 4.0.9

- Support for Proxy Settings

## 4.0.0

- IPInfo not supported on Splunk 6.x and 7.x

## 3.5.4

- Bugfixes : Issues with ipinfolookup command

## 3.5.3

- Added Support for New Lookup Commands: `privacyinfolookup`,
`domaininfolookup` and `rangesinfolookup`.

## 3.4.11

- Bug Fixes and Compliance to Splunk App Inspect

## 3.4.9

- New scripted lookup
- New ipinfobatch command

## 3.0.0

- Support to Splunk 8.x and Python 3.x

## 1.0.7

- Bug Fixes
- Color Issues

## 1.0.3

- Replace old dashboard screen with new

## 1.0.2

- Added Screenshots and Web Installation Steps

## 1.0.0

- Initial Version

