project(npotokendemo)

cmake_minimum_required(VERSION 3.11)
set(EOSIO_WASM_OLD_BEHAVIOR "Off")
find_package(eosio.cdt)

add_contract( npotokendemo npotokendemo npotokendemo.cpp )
target_include_directories( npotokendemo PUBLIC ${CMAKE_SOURCE_DIR}/../include )