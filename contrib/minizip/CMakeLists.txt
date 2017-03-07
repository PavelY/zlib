#
# minizip
#
fips_begin_lib(minizip)
    fips_files(
        crypt.h
        ioapi.h ioapi.c
        miniunz.c
        mztools.h mztools.c
        unzip.h unzip.c
        zip.h zip.c
    )
    add_definitions(-D_NO_FSEEKO)
    add_definitions(-D_CRT_SECURE_NO_DEPRECATE)
    add_definitions(-D_CRT_NONSTDC_NO_DEPRECATE)
fips_end_lib(zlib)
