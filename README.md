# SevenZip

SevenZip is an Objective-C wrapper framework around [p7zip](http://p7zip.sourceforge.net/), which in turn is a Unix port of [7zip](http://www.7-zip.org/). 

### Building

1. clone this repo
2. get the p7zip sources from [http://sourceforge.net/projects/p7zip/](http://sourceforge.net/projects/p7zip/)
3. copy the contents of the `p7zip_XX.YY` folder into `<repo_root>/External/p7zip`
4. open the Xcode project and build the `SevenZip` target

If you just want to toy with it, take a look at the `SVZTest` app (separate target).

### Disclaimer

At the moment, the wrapper is in very early stage of development but you can already create 7z archives from code without having to wet your feet with the underlying MFC/COM+/OLE/godknowswhat implementation. (I accept donations for funding my therapy to get over the shock of dealing with that code. With all due respect.)