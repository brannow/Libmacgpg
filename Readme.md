Libmacgpg
=========

Libmacgpg is an Objective-C framework which makes it easier to communicate with gnupg.
It's the base framework for all apps and services of [GPG Suite](https://gpgtools.org)

Updates
-------

The latest releases of Libmacgpg is part of GPG Suite and can be found on our [official website](https://gpgtools.org).

For the latest news and updates check our [Twitter](https://twitter.com/gpgtools).

If you have any questions how to use Libmacgpg in your own App, contact us on our [support page](https://gpgtools.tenderapp.com).


Build
-----

#### Clone the repository
```bash
git clone --recursive https://github.com/GPGTools/Libmacgpg.git
cd Libmacgpg
```

make sure you are in the correct branch 
```bash 
git branch
```
for example to checkout the dev branch
```bash 
git fetch --all
git checkout dev
```

#### Build
```bash
make
```

#### Install
To install Libmacgpg copy build/Release/Libmacgpg.framework into the framework folders.
best way is to install the Trail Version of GPG Suite it will install the framework for you and will enable the xps service.
We simply replace the Licance Framework with the opensource Version

```bash
cp -R ./build/Release/Libmacgpg.framework ~/Library/Frameworks/Libmacgpg.framework
```

and

```bash
cp -R ./build/Release/Libmacgpg.framework /Library/Frameworks/Libmacgpg.framework
```

You might need for Mojave to enable the Terminal to access the Framework directories in System settings > Security -> Privacy.
"Full Access"  add the Terminal.app under /Applications/Utilities

Enjoy your custom Libmacgpg.


System Requirements
-------------------

* Mac OS X >= 10.6
* GnuPG v2.0.26

tested on Mac OS X Mojave 10.14 (18A391) and Apple Mail Version 12.0 (3445.100.39)
