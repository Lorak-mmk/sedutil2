target_sources(sedutil2-cli
        PRIVATE
            DtaDevLinuxDrive.h
            DtaDevLinuxNvme.h
            DtaDevLinuxNvme.cpp
            DtaDevLinuxSata.h
            DtaDevLinuxSata.cpp
            DtaDevOS.h
            DtaDevOS.cpp
            os.h)

target_include_directories(sedutil2-cli PRIVATE .)