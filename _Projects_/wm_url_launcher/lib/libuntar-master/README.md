# libuntar

This library provides `.tar`, `.tar.gz` (GZip), and `.tar.bz2` (BZip2) archive handling and extraction to the PlayStation 3 using the [PSL1GHT SDK](https://github.com/ps3dev/PSL1GHT/).

## Source Version

 - libbzip2 [1.0.6](https://github.com/bucanero/psl1ght-libs/tree/master/bzip2)
 - based on [untar.c](https://github.com/libarchive/libarchive/blob/master/contrib/untar.c)

### Exports

 - untar(): extracts contents from a .tar uncompressed archive
 ```c
int untar(const char* srcFile, const char* dstPath);
 ```
 - untar(): extracts contents from a .tar.gz (GZip) compressed archive
 ```c
int untar_gz(const char* srcFile, const char* dstPath);
 ```
 - untar_bz2(): extracts contents from a .tar.bz2 (BZip2) compressed archive
 ```c
int untar_bz2(const char* srcFile, const char* dstPath);
 ```

## Build/Install

Build the library with: 
```
make
```

Install the library to your PSL1GHT setup with:
```
make install
```

## Documentation

 - [BZip2 manual](https://github.com/bucanero/psl1ght-libs/blob/master/bzip2/manual.pdf)

## Sample app

You can find a sample PSL1GHT app using the library [here](./example).

## License

`libuntar` is released under the [MIT License](./LICENSE).