
cmake_minimum_required(VERSION 2.8)

project(hellobullet)

include_directories(/usr/local/include/bullet)

link_directories(/usr/local/lib)

#add_definitions(-D)

add_executable(hellobullet hellobullet.cpp)

target_link_libraries(hellobullet BulletSoftBody BulletDynamics BulletCollision LinearMath)

# libBulletCollision.a
# libBulletDynamics.a
# libBulletMultiThreaded.a
# libBulletSoftBody.a
# libBulletSoftBodySolvers_CPU.a
# libBulletSoftBodySolvers_OpenCL_Mini.a
# libLinearMath.a
