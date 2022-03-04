cmake_minimum_required(VERSION 3.15)
project(word2vec_commented C)

set(CMAKE_C_STANDARD 11)
#set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -lm -pthread -O3 -march=native -Wall -funroll-loops -Wno-unused-result")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -lm -pthread -O0 -march=native -Wall -funroll-loops -Wno-unused-result")

add_executable(word2vec_commented
#        compute-accuracy.c
#        distance.c
#        word-analogy.c
#        word2phrase.c
        word2vec.c
        )
target_link_libraries(word2vec_commented m)