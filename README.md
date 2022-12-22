# Windows-Backup-Scripts

A collection of scripts that I use to backup my Windows laptop.

The first script is the simple and stupid script. It just makes a tar file of every file on my hard drive that I care about.

The second script is smarter. It checks for files that have changed since the last backup, filters out the ones that I don't care about, further filters out
those files that have been modified since when the copy on the backup drive was last modified, and only copies the ones that pass all of the filtering. The same
filtering applies to directories, except that the script *creates* copies of directories on the backup drive, rather than copying the entire directory.