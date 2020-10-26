target_sources(sedutil2-cli
        PRIVATE
            bitops.h
            blockwise.h
            blockwise.c
            chash.h
            chash.c
            handy.h
            hmac.h
            hmac.c
            pbkdf2.h
            pbkdf2.c
            sha2.h
            sha512.c
            tassert.h)

target_include_directories(sedutil2-cli PRIVATE .)