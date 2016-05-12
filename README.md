cfengine-snippets
=================

Policy snippets for cfengine 3.x

These are little stand-alone policies that can be placed into the 
masterfiles/services/autorun/ directory.  They offer a quick starting point
to a new cfengine user for some commonly-used tasks.

They can be run as standalone executables, also.  Just run ./<policy>.cf [-KIv]

Policy Descriptions
------------------
* set_root_password.cf - Take the hash in the policy file, and make sure that the root user has that as their password hash.  The default password is "vagrant", which should be changed to your password hash.
* cfengine_motd.cf - Put some information about cfengine into /etc/motd
* system_standard_pkgs.cf - Install some standard packages, and illustrate how package version promises are handled
* remove_bigfile.cf - Watch for (log) files that are over a particular size and truncate them
* onetime.cf - Run a command once per system lifecycle (or as long as a flag file exists)
