include_directories(includes)

add_subdirectory(basic)
add_subdirectory(official)

# memory access
add_subdirectory(testMisaligned)

# interrupts and events
add_subdirectory(testEvents)
add_subdirectory(testExceptions)

# arithmetic operations
add_subdirectory(testALU)
add_subdirectory(testALUExt)
# disabled for now since opcodes clash
add_subdirectory(testMUL)

# ETH specific features
add_subdirectory(testBitManipulation)
add_subdirectory(testCnt)
add_subdirectory(testClip)
add_subdirectory(testVecArith)
add_subdirectory(testVecCmp)

add_subdirectory(testDivRem)
add_subdirectory(testShufflePack)
add_subdirectory(testAddSubNorm)
add_subdirectory(testMacNorm)
add_subdirectory(testDotMul)

# other core features
add_subdirectory(testCSR)

# add_subdirectory(testDebug)

add_subdirectory(debug)
