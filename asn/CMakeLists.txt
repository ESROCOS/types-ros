# H2020 ESROCOS Project
# Company: GMV Aerospace & Defence S.A.U.
# Licence: GPLv2

file(GLOB ASN1_SOURCES RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} "*.asn")

esrocos_asn1_types_package(esrocos_types_ros
    ${ASN1_SOURCES}
)

esrocos_asn1_types_build_test(esrocos_types_ros)
esrocos_asn1_types_install(esrocos_types_ros ${CMAKE_INSTALL_PREFIX}/types/ros)

