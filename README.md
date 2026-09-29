# Shane Dabirsiaghi

Principal Software Engineer and founding engineer at Contrast Security. I build
runtime instrumentation and security systems: CLR internals and IL rewriting,
Windows kernel drivers, process attachment and injection, and eBPF-based workload
visibility on Linux, in C++, Rust, and C#.

Co-inventor on [US Patent 11,222,122](https://patents.google.com/patent/US11222122):
Method and System for Runtime Instrumentation of Software Methods.

## Upstream contributions

**[microsoft/CLRInstrumentationEngine](https://github.com/microsoft/CLRInstrumentationEngine)**

Microsoft's cooperative profiler for running multiple .NET profilers in one process.

- [#303](https://github.com/microsoft/CLRInstrumentationEngine/pull/303): Fixed
  stack-depth calculation for calls to generic methods. The engine used the
  MethodSpec signature, which encodes only generic arguments, producing a too-low
  maxStack and InvalidProgramException in instrumented applications.
- [#278](https://github.com/microsoft/CLRInstrumentationEngine/pull/278): Reused the
  existing AssemblyInfo in AssemblyLoadFinished instead of creating a new one that
  overwrote the instance already registered during ModuleLoadFinished.
- [#276](https://github.com/microsoft/CLRInstrumentationEngine/pull/276): Fixed
  AssemblyInfo::GetModules, which always returned a NULL IEnumModuleInfo.

**[microsoft/elfcore](https://github.com/microsoft/elfcore)**

Rust crate for creating core dumps of running Linux processes.

- [#39](https://github.com/microsoft/elfcore/pull/39): Fixed the aarch64 build of
  the Linux ptrace path, added ARM64 CI builds and tests, and updated tests for
  aarch64 register layouts.

## Side projects

- [PearlHq](https://github.com/m0nkey653/PearlHq): Pet food and water sensors on an
  Adafruit Feather ESP32-C6, with a backend and web UI.
- [SpaceViewportStudio](https://github.com/m0nkey653/SpaceViewportStudio): Generates
  deep-space panoramas spanning linked Lian Li TL LCD case fans.
- [ClueSnake](https://github.com/m0nkey653/ClueSnake): Snake on the Adafruit CLUE
  (nRF52840) in C++.
- [PwnNetShell](https://github.com/m0nkey653/PwnNetShell): ASP.NET web shell built
  for authorized penetration testing engagements at Aspect Security (circa 2012).

## Elsewhere

[LinkedIn](https://linkedin.com/in/shane-dabirsiaghi)
