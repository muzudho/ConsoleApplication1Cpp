# プロジェクトルートにある external/spdlog/include をインクルードパスに追加
target_include_directories(ConsoleApplication1Cpp PRIVATE
    ${CMAKE_SOURCE_DIR}/external/spdlog/include
)