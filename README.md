# About

[![License][license-badge]][license]

After deploying several Windows Virtual Desktop environments I decided I no longer wanted to manually download the Admx files I needed, and I wanted a way to keep them up-to-date.

This script solves both problems.
* Checks for newer versions of the Admx files that are present and processes the new version if found
* Optionally copies the new Admx files to the Policy Store or Definition folder, or a folder of your chosing

The name I chose for this script is an ode to the Evergreen module (https://github.com/aaronparker/Evergreen) by Aaron Parker (@stealthpuppy).

# How to use

Quick start:
* Download the script to a location of your chosing (for example: C:\Scripts\EvergreenAdmx)
* Run or schedule the script

I have scheduled the script to run daily using the following command:

`
EvergreenAdmx.ps1 -WindowsVersion "20H2" -PolicyStore "C:\Windows\SYSVOL\domain\Policies\PolicyDefinitions"
`

[github-release-badge]: https://img.shields.io/github/release/msfreaks/EvergreenAdmx.svg?style=flat-square
[github-release]: https://github.com/msfreaks/EvergreenAdmx/releases/latest
[license-badge]: https://img.shields.io/github/license/msfreaks/EvergreenAdmx.svg?style=flat-square
[license]: https://github.com/msfreaks/EvergreenAdmx/blob/master/LICENSE

