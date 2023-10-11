# Awesome Code Coverage

A curated list of code coverage resources. Only free tools are included.

#### What is code coverage?
> Code coverage is the process of measuring the percentage of the source code lines that are executed during testing.

Commonly, code coverage tools are implemented by these ways.

- Instrumentation at compile time, insert addtional codes to collect code coverage.
- Act as a debugger, insert break points at runtime, collect code coverage.
- Use existing instrumetation/debug interface provided by the language, collect code coverage (e.g., Lua, Python).

## Contents
- [Tools](#tools)
- [Documentations](#Documentations)
- [Papers](#papers)
- [Blogs](#blogs)
  
## Tools
### C & C++
| Tools | Supported OS | Implementation | Branch Coverage |
| :-----: | :----------: | :------------: | :---------------: |
| [gcov](https://gcc.gnu.org/onlinedocs/gcc/Gcov.html) | All OS supported by gcc | Instrumentation | YES |
| [kcov](https://github.com/SimonKagstrom/kcov) | FreeBSD/Linux/MacOS | Debugger | NO |
| [OpenCppCoverage](https://github.com/OpenCppCoverage/OpenCppCoverage) | Windows | Debugger | NO |

### Go
| Tools | Supported OS | Implementation | Branch Coverage |
| :-----: | :----------: | :------------: | :---------------: |
| go cover | All OS supported by Go | Instrumentation | NO |
| [goc](https://github.com/qiniu/goc) | All OS supported by Go | Instrumentation | NO |
| [gobco](https://github.com/rillig/gobco) | All OS supported by Go | Instrumentation | YES |
| [kcov](https://github.com/SimonKagstrom/kcov) | FreeBSD/Linux/MacOS | Debugger | NO |

### Java
| Tools | Supported OS | Implementation | Branch Coverage |
| :-----: | :----------: | :------------: | :---------------: |
| [JaCoCo](https://www.jacoco.org/jacoco/trunk/index.html) | All OS supported by JVM | Instrumentation (at runtime by java agent) | YES |
| [cobertura](https://github.com/cobertura/cobertura) | All OS supported by JVM | Instrumentation| YES |

### Smali
| Tools | Supported OS | Implementation | Branch Coverage |
| :-----: | :----------: | :------------: | :---------------: |
| [acvtool](https://github.com/pilgun/acvtool) | Android | Instrumentation | NO |

### Lua
| Tools | Supported OS | Implementation | Branch Coverage |
| :-----: | :----------: | :------------: | :---------------: |
| [luacov](luacov) | All OS supported by Lua | Debug Interface (debug module) | Partial |

### Documentations
* [LLVM - Source-based Code Coverage](https://clang.llvm.org/docs/SourceBasedCodeCoverage.html)
  
## Papers
* [Smali - Fine-grained code coverage measurement in automated black-box Android testing](https://satoss.uni.lu/members/sjouke/papers/PGZDKM20.pdf)

## Blogs
* [Go - Coverage profiling support for integration tests](https://tip.golang.org/testing/coverage/)
* [What is Wrong with Statement Coverage](https://www.bullseye.com/statementCoverage.html)