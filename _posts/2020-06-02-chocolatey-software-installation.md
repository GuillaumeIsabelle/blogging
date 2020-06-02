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
> Packaging

Source: *[Chocolatey Software | Installation][1]*

<!-- wp:code -->

<pre class="wp-block-code"><code># Set directory for installation - Chocolatey does not lock
# down the directory if not the default
$InstallDir='C:\ProgramData\chocoportable'
$env:ChocolateyInstall="$InstallDir"

# If your PowerShell Execution policy is restrictive, you may
# not be able to get around that. Try setting your session to
# Bypass.
Set-ExecutionPolicy Bypass -Scope Process -Force;

# All install options - offline, proxy, etc at
# https://chocolatey.org/install
iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
</code></pre>

<!-- /wp:code -->

 [1]: https://chocolatey.org/docs/installation#non-administrative-install