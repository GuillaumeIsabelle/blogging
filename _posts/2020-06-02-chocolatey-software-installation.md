---
ID: 1993
post_title: Chocolatey Software | Installation
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2020/06/02/chocolatey-software-installation/
published: true
post_date: 2020-06-02 12:44:01
---
> try { # Set TLS 1.2 (3072) as that is the minimum required by Chocolatey.org # Use integers because the enumeration value for TLS 1.2 won't exist # in .NET 4.0, even though they are addressable if .NET 4.5+ is # installed (.NET 4.5 is an in-place upgrade). [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072 } catch { Write-Warning 'Unable to set PowerShell to use TLS 1.2. This is required for contacting Chocolatey as of 03 FEB 2020. h Source: *[Chocolatey Software | Installation][1]*

 [1]: https://chocolatey.org/docs/installation#non-administrative-install