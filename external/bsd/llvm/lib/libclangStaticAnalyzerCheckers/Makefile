#	$NetBSD: Makefile,v 1.26 2017/01/11 12:02:32 joerg Exp $

LIB=	clangStaticAnalyzerCheckers

.include <bsd.init.mk>

.PATH: ${CLANG_SRCDIR}/lib/StaticAnalyzer/Checkers
.PATH: ${CLANG_SRCDIR}/lib/StaticAnalyzer/Checkers/MPI-Checker

SRCS+=	AllocationDiagnostics.cpp \
	AnalysisOrderChecker.cpp \
	AnalyzerStatsChecker.cpp \
	ArrayBoundChecker.cpp \
	ArrayBoundCheckerV2.cpp \
	BasicObjCFoundationChecks.cpp \
	BlockInCriticalSectionChecker.cpp \
	BoolAssignmentChecker.cpp \
	BuiltinFunctionChecker.cpp \
	CXXSelfAssignmentChecker.cpp \
	ClangCheckers.cpp \
	CStringChecker.cpp \
	CStringSyntaxChecker.cpp \
	CallAndMessageChecker.cpp \
	CastSizeChecker.cpp \
	CastToStructChecker.cpp \
	CheckObjCDealloc.cpp \
	CheckObjCInstMethSignature.cpp \
	CheckSecuritySyntaxOnly.cpp \
	CheckSizeofPointer.cpp \
	CheckerDocumentation.cpp \
	ChrootChecker.cpp \
	CloneChecker.cpp \
	ConversionChecker.cpp \
	DeadStoresChecker.cpp \
	DebugCheckers.cpp \
	DereferenceChecker.cpp \
	DirectIvarAssignment.cpp \
	DivZeroChecker.cpp \
	DynamicTypeChecker.cpp \
	DynamicTypePropagation.cpp \
	ExprInspectionChecker.cpp \
	FixedAddressChecker.cpp \
	GTestChecker.cpp \
	GenericTaintChecker.cpp \
	IdenticalExprChecker.cpp \
	IteratorPastEndChecker.cpp \
	IvarInvalidationChecker.cpp \
	LLVMConventionsChecker.cpp \
	LocalizationChecker.cpp \
	MPIBugReporter.cpp \
	MPIChecker.cpp \
	MPIFunctionClassifier.cpp \
	MacOSKeychainAPIChecker.cpp \
	MacOSXAPIChecker.cpp \
	MallocChecker.cpp \
	MallocOverflowSecurityChecker.cpp \
	MallocSizeofChecker.cpp \
	NSAutoreleasePoolChecker.cpp \
	NSErrorChecker.cpp \
	NoReturnFunctionChecker.cpp \
	NonNullParamChecker.cpp \
	NullabilityChecker.cpp \
	NumberObjectConversionChecker.cpp \
	ObjCAtSyncChecker.cpp \
	ObjCContainersASTChecker.cpp \
	ObjCContainersChecker.cpp \
	ObjCMissingSuperCallChecker.cpp \
	ObjCPropertyChecker.cpp \
	ObjCSelfInitChecker.cpp \
	ObjCSuperDeallocChecker.cpp \
	ObjCUnusedIVarsChecker.cpp \
	PaddingChecker.cpp \
	PointerArithChecker.cpp \
	PointerSubChecker.cpp \
	PthreadLockChecker.cpp \
	RetainCountChecker.cpp \
	ReturnPointerRangeChecker.cpp \
	ReturnUndefChecker.cpp \
	SimpleStreamChecker.cpp \
	StackAddrEscapeChecker.cpp \
	StdLibraryFunctionsChecker.cpp \
	StreamChecker.cpp \
	TaintTesterChecker.cpp \
	TestAfterDivZeroChecker.cpp \
	TraversalChecker.cpp \
	UndefBranchChecker.cpp \
	UndefCapturedBlockVarChecker.cpp \
	UndefResultChecker.cpp \
	UndefinedArraySubscriptChecker.cpp \
	UndefinedAssignmentChecker.cpp \
	UnixAPIChecker.cpp \
	UnreachableCodeChecker.cpp \
	VLASizeChecker.cpp \
	ValistChecker.cpp \
	VforkChecker.cpp \
	VirtualCallChecker.cpp

.include "${.PARSEDIR}/../../tablegen.mk"

.if defined(HOSTLIB)
.include <bsd.hostlib.mk>
.else
.include <bsd.lib.mk>
.endif
