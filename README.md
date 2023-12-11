# These two scripts are useful for sharing files using curl to a null server that is 0x0.st (curl -F"file=@filename.txt" 0x0.st)

**After uploading file to that null server we will get a url from which we can download that file using wget**

**upfile** script is simple script which will upload files without any password

**supfile** script encrypts + zip that file with password (user provides password)

**You need to have uuid-runtime package for supfile script to work so install it using `sudo apt install uuid-runtime`**

For making it easy add these two scripts to `/usr/local/bin`and make it executable using chmod + x so that you can access it from anywhere in system. 

**When you will download files using `supfile` and then unzip that zip file, it will automatically create a tmp folder inside ur file system and inside that tmp folder will be a unique a `uuid` and inside that uuid will be ur file . 
