cmake_minimum_required(VERSION 3.24)

set(Boost_NO_WARN_NEW_VERSIONS ON)

project(
  EcosystemOfServices
)

find_package(
  cpprestsdk
    CONFIG REQUIRED
)

find_package(
  bsoncxx
    CONFIG REQUIRED
)

find_package(
  mongocxx
    CONFIG REQUIRED
)

find_package(
  cpp-jwt
    CONFIG REQUIRED
)

add_subdirectory(InvestorService)

add_subdirectory(ApiGatewayService)

add_subdirectory(AuthenticationService)
