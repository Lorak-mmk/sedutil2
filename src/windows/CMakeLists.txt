target_sources(sedutil2-cli
        PRIVATE
            DtaDevOS.h
            DtaDevOS.cpp
            DtaDiskATA.h
            DtaDiskATA.cpp
            DtaDiskNVMe.h
            DtaDiskNVMe.cpp
            DtaDiskUSB.h
            DtaDiskUSB.cpp
            os.h)

target_include_directories(sedutil2-cli PRIVATE .)