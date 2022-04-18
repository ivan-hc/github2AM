# GitHub To "AM" (github2AM)
A script to convert apps from Github to installation scripts for "AM" Application Manager.

### INSTALL
Use "AM" to install this script, run the command:

    sudo am -i github2am
    
### UNINSTALL
With "AM":

    sudo am -r github2am
Without "AM":

    sudo /opt/github2am/remove

### USAGE
    github2am convert $USER/$REPO
where `$USER/$REPO` is the name of the repository where the app is stored.

For more alternative templates, see the `-t` option of the main project, ie "AM" Application Manager.

This script supports multiple arguments, so you can create multiple templates.

### TEST
All you have to test is the download of the application. During the download you can always press CTRL+C to abort.
Create a new empty folder and run the scripts there in a terminal window (the script will create a `tmp` and `icons` folder):
- if `wget` is downloadinding what you need (for example an AppImage), the script works as expected;
- if `wget` is not downloading what you need (maybe an AppImage for different architectures), then edit the created script (maybe the lines 28 and 54, or just the line 11) and try again.

## This script is part of [ivan-hc/AM-Application-Manager](https://github.com/ivan-hc/AM-Application-Manager).
