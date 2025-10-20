set(WRECEIVER_SOURCES
    wReceiver.cpp
)

add_executable(wReceiver ${WRECEIVER_SOURCES})

target_link_libraries(wReceiver PRIVATE cxxopts::cxxopts spdlog::spdlog Boost::regex common)
target_include_directories(wReceiver PRIVATE ${PROJECT_SOURCE_DIR}/common)