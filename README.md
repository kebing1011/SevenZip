# SevenZip ![](https://www.bitrise.io/app/4d43df2229198af5.svg?token=upgdQ6LNU-RCnL8rdhsq7A)

SevenZip is an Objective-C wrapper framework around [p7zip](http://p7zip.sourceforge.net/), which in turn is a Unix port of [7zip](http://www.7-zip.org/). 

### Requirements

Xcode 6, OSX 10.9, iOS 8.4

(It probably builds on earlier platform versions as well but I didn't care enough to check.)

### Building

1. clone this repo
2. from the repo root, run

    ```
    $ scripts/setup.sh
    ```
    
3. open the Xcode project and build the `SevenZip (OSX)`/`SevenZip (iOS)` target

If you just want to toy with it, take a look at the `SVZDemo`/`SVZDemo-iOS` apps (separate targets).

### Features

- listing the archive contents
inside
- extracting all/some files from archives to file/memory
- **creating** new archives with files/directories 
- **adding/removing** files to/from existing archives

Coming soon: proper password handling, [tests](https://github.com/lvsti/SevenZip/tree/master/SevenZipTests), automated builds, [documentation](https://github.com/lvsti/SevenZip/wiki), free candy/beer. Until then, submit your requests/bug reports as [issues](https://github.com/lvsti/SevenZip/issues).

### Disclaimer

At the moment, the project is still in an early stage of development but you can already do all the usual stuff with 7z archives from code without having to get your hands dirty with the underlying MFC/COM+/OLE/godknowswhat implementation.

Be warned that the code is experimental, has few tests, and is provided as-is. Be prepared for unwanted/undefined behavior, data losses, nazgul attacks etc.

### Credits

- the guy behind [p7zip](http://sourceforge.net/projects/p7zip/), for doing the lion's share of porting
- Oleh Kulykov's [LzmaSDK-ObjC](https://github.com/OlehKulykov/LzmaSDK-ObjC) for some inspiration about implementing custom streams
- pixelglow's [ZipZap](https://github.com/pixelglow/ZipZap) for their API I shamelessly copied
