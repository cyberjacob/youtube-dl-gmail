# Gmail intigration for youtube-dl

youtube-dl-gmail is a script designed to be run as a cronjob that automatically fetches "<user> just uploaded a video" messages from a specific label in Gmail and queues them for download.
To reduce bandwidth, usage, only one video is downloaded each time the script is run.
Emails are automatically moved to the trash folder once they have been scanned and queued for downloading.
Status is displayed in the process title, visible through `ps -Af | grep gmail` or `cat /proc/pid/cmdline`
Currently, the script is only capable of retreiving videos from YouTube.

