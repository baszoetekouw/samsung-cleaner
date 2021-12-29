# samsung-cleaner
Remove Samsung bloatware from android phones.

If you would like to debloat your Samsung hone, you are probably better off using the [Universal Android Debloater](https://github.com/0x192/universal-android-debloater).

However, I was too lazy to get a nightly version of Rust to work on my laptop, so I wrote this instead.  I mostly used the info from UAD (https://github.com/0x192/universal-android-debloater/blob/main/resources/assets/uad_lists.json) to determine what to remove.

## How to use this
- Install adb
- Connect you phone to adb (make sure it is listed exactly once by `adb devices`)
- run the script
- it will list all packages that are installed on you phone (but will remove nothing yet)
- it will write two scripts `do_remove.sh` and `do_restore.sh` 
- run `do_remove.sh` to actually remove the bloatware.
