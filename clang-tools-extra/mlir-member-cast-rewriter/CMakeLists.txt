set(LLVM_LINK_COMPONENTS support)

add_clang_executable(mlir-member-cast-rewriter
  mlir-member-cast-rewriter.cpp
  )
target_link_libraries(mlir-member-cast-rewriter
  PRIVATE
    clangAST
    clangBasic
    clangFormat
    clangFrontend
    clangLex
    clangRewrite
    clangSerialization
    clangTooling
    clangToolingCore
    clangToolingRefactoring
  )
