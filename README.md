# slitaz-wok
Receipts for Slitaz

## Set up your SliTaz development environment

1. Install the development package and it’s dependencies with the following command:
```bash
# tazpkg -gi tazdev
```

2. Create the isolated chroot environment for development:
```bash
# tazdev -gc
# su
```

3. chroot to the development environment:
```bash
# tazdev chroot
```

4. Install the utilities needed to start cooking:
```bash
# tazpkg recharge
# tazpkg -gi cookutils
```

5. Clone the wok repository or create one for personal use:
```bash
# cook setup --wok //clone the wok to build official packages
OR
# cook setup //create a wok from scratch for personal use
```
6. cd to /home/slitaz and cook the slitaz-doc package as a start:
```bash
# cd /home/slitaz
# cooker pkg slitaz-doc
```

You will find the package created under the /home/slitaz/packages directory.
8. The downloaded source packages and source code for the packages will be present under the src and wok directories. cd around to get accustomed to various directories and files.



## License

This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details
