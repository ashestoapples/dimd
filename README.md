# dimd
# Duplicate IMage Detector

This script will find visually similar images in the users image directories (specified in the config file). Dimd will log a md5 hash of each original image in a database file (located in /home/user/.dimd). 

Make the script usable first (chmod +x dimd) then when you first run this script pass "dimd --init" to create the .dimd folder in your home directory and generate the default config file. Put the dimd file in your path for easy execution.

Pass '-h' or '--help' for a summary of the arguments

The hashing algorithm is based off of this article: http://blog.iconfinder.com/detecting-duplicate-images-using-python/

I figured I'd make something usefull for myself (and hopefully others) with it. 

# TODO:
Preferred directories
Windows Support
Windows GUI

# Config file syntax:

Comments are made with '!'
'large' and 'small' denote wether bigger (higher res) or smaller (lower res) images are preferred by the script

Having 'logDeletes' in the config file will cause the script to wirte a log of which user ran it, and when files were deleted by it

'dirs
{
  /path/to/imgs
  /path/to/porn
}'  specefy dirs checked by dimd

'ignored
{
  /path/to/imgs/sub
}'  sub directories for dimd to ignore, you MUST include the preceeding path to the sub dir

'formats
{
  .jpg
  .png
}'  image formats dimd will recognize
