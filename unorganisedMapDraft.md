Prefixes:
KDDK => Ke
NAPI =>  N
Runtime Library => Rtl

Style: PascalCase

ExitProcess => RtlExitUserProcess => NTerminateCurrentProcess

VirtualAlloc => NAllocateVirtualMemory
HeapAlloc => RtlHeapAlloc (it can call NAllocateVirtualMemory, but doesn't have to)

CreateFile => NCreateFile
CloseHandle => NCloseHandle

Etc etc

Abbreviations/terminology:
KDDK => Kernel Driver Development Kit
NAPI => Native API
UNAPIM => Usermode Native API Mapping
Rtl => Runtime Library
KM => Kernel Mode
UM => User Mode

Abstract apis:
KDDK => Kernel Driver Development Kit
NAPI => Native API
UNAPIM => Usermode Native API Mapping
Rtl => Runtime Library 
Utility.dll => set of "exposed" friendly API interfaces, basically abstraction and collection of Rtl/UNAPIM
kernel.exe => Dynamically linked kernel mode entries (primarily used for KDDK)
Kernel architecture: Hybrid
Syscalls model => dynamic, varies from version to version
Type => A graphical system with windows and graphical user interfaces
License => proprietary
