#	$NetBSD: Makefile,v 1.13 2017/01/11 12:02:27 joerg Exp $

PROG_CXX=	llvm-objdump
NOMAN=		yes

.include <bsd.init.mk>

.PATH: ${LLVM_SRCDIR}/tools/llvm-objdump

SRCS=	llvm-objdump.cpp \
	COFFDump.cpp \
	ELFDump.cpp \
	MachODump.cpp \
	WasmDump.cpp

LLVM_LIBS+= \
	AArch64Disassembler \
	AArch64AsmParser \
	AArch64MCTargetDesc \
	AArch64AsmPrinter \
	AArch64TargetInfo \
	AArch64Utils \
	ARMDisassembler \
	ARMAsmParser \
	ARMMCTargetDesc \
	ARMAsmPrinter \
	ARMTargetInfo \
	MipsDisassembler \
	MipsAsmParser \
	MipsMCTargetDesc \
	MipsAsmPrinter \
	MipsTargetInfo \
	PowerPCDisassembler \
	PowerPCAsmParser \
	PowerPCMCTargetDesc \
	PowerPCAsmPrinter \
	PowerPCTargetInfo \
	SparcDisassembler \
	SparcAsmParser \
	SparcMCTargetDesc \
	SparcAsmPrinter \
	SparcTargetInfo \
	X86Disassembler \
	X86AsmParser \
	X86CodeGen \
	X86MCTargetDesc \
	X86AsmPrinter \
	X86TargetInfo \
	X86Utils \
	CodeGen \
	MCDisassembler \
	DebugInfoDWARF \
	DebugInfoSymbolize \
	DebugInfoPDB \
	DebugInfoPDBRaw \
	Object \
	BitReader \
	MCParser \
	MC \
	IR \
	Support \
	Demangle

LDADD+=	-lz
DPADD+=	${LIBZ}

.include "${.PARSEDIR}/../../link.mk"

.include <bsd.prog.mk>
