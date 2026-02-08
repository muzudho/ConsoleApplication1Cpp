cmake_minimum_required(VERSION 3.15)  # 古くてもOKだけど最近のほうがいい

project(ConsoleApplication1Cpp)

# spdlog の include パスを追加（${CMAKE_SOURCE_DIR} はプロジェクトルート）
target_include_directories(${PROJECT_NAME} PRIVATE
    ${CMAKE_SOURCE_DIR}/external/spdlog/include
)

# 実行ファイルの定義（.cppファイルはここに全部書くか、add_executable の第2引数以降に）
add_executable(${PROJECT_NAME}
    ConsoleApplication1Cpp.cpp
    LoggingExample.cpp   # もしこれもコンパイル対象なら
)

