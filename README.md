moodle-download
=======
Moodle downloader modified to work with Birkbeck Moodle

Installation
------------

1. Download or clone the repository from GitHub.
2. Install the requirements: `sudo easy_install pip
sudo pip install -r requirements.txt`
3. Create necessary directories: `mkdir -p ~/.config/moodle-download/profiles`
4. Copy your configuration file to `nano ~/.config/moodle-download/moodle-download.conf` 
5- run it `python /Applications/MAMP/htdocs/pg/moodle-download/moodle-download/moodle-download.py WS-2015-2016`

Profiles
------------

All profile files must be valid JSON files. For every course you take, add a new dictionary to the profile. The key should be the course title (but doesn't really matter), `id` is the Moodle course id (see URL of overview page), `short` is a short description that will be used for symlinks, and `downloads` lists the files to download. The first element is a regular expression that should match the files to download, second specifies the rename pattern and the third determines the download location.


License
-------

**GNU General Public License (GPLv3)**, see `LICENSE.txt` for further details.
