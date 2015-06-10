This is a repo manifest for testing libsel4thrds.

Basic instructions:

Install repo, for instance:
```
mkdir -p ~/bin
export PATH=~/bin:$PATH
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
```
And then create a directory for the project and then init and synchronize
(Note: we currently need the repo master branch to handle wildcards):
```
mkdir test-thrds
cd test-thrds
repo init --repo-branch=master -u https://github.com/winksaville/sel4-test-thrds-manifest.git
repo sync
```
You can ignore the clone.bundle errors, see below
```
curl: (22) The requested URL returned error: 404 Not Found
Server does not provide clone.bundle; ignoring.
```
