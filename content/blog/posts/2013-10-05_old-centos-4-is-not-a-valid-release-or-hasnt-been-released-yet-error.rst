Old CentOS "4 is not a valid release or hasnt been released yet" error
######################################################################
:date: 2013-10-05 09:52
:author: Stefano
:category: Linux
:tags: centos
:slug: old-centos-4-is-not-a-valid-release-or-hasnt-been-released-yet-error

If you have to handle an old Centos 4 machine and you try to use yum to
get some packages, you will get an error "4 is not a valid release or
hasnt been released yet". This is because CentOS 4 is end of life, and
the default repo does not provide updates anymore. Yet, you might still
be interested in getting the latest packages for the end of life
release.

You can solve the problem by switching to the vault as a repo, doing the
following

#. open /etc/yum.repos.d/CentOS-Base.repo
#. comment out all the mirrorlist entries
#. uncomment and set all the baseurl entries to
   http://vault.centos.org/4.9/os/$basearch


