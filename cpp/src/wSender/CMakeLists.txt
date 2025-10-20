set(WSENDER_SOURCES
    wSender.cpp
)

add_executable(wSender ${WSENDER_SOURCES})

target_link_libraries(wSender PRIVATE cxxopts::cxxopts spdlog::spdlog Boost::regex common)
target_include_directories(wSender PRIVATE ${PROJECT_SOURCE_DIR}/common)