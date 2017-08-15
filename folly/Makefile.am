if FOLLY_TESTMAIN
MAYBE_INIT = init
endif

# Note that the order of SUBDIRS matters.
# Many subdirectories depend on libfollytest from the test directory,
# so it must appear before other directories
SUBDIRS = . test experimental $(MAYBE_INIT) io/test stats/test

ACLOCAL_AMFLAGS = -I m4

CLEANFILES =


noinst_PROGRAMS = generate_fingerprint_tables
generate_fingerprint_tables_SOURCES = build/GenerateFingerprintTables.cpp
generate_fingerprint_tables_LDADD = libfollybase.la

noinst_LTLIBRARIES = \
	libfollybasesse42.la \
	libfollybase.la

lib_LTLIBRARIES = \
	libfolly.la \
	libfollybenchmark.la

follyincludedir = $(includedir)/folly

nobase_follyinclude_HEADERS = \
	ApplyTuple.h \
	Arena-inl.h \
	Arena.h \
	Array.h \
	Assume.h \
	AtomicBitSet.h \
	AtomicHashArray-inl.h \
	AtomicHashArray.h \
	AtomicHashMap-inl.h \
	AtomicHashMap.h \
	AtomicIntrusiveLinkedList.h \
	AtomicLinkedList.h \
	AtomicStruct.h \
	AtomicUnorderedMap.h \
	Baton.h \
	Benchmark.h \
	Bits.h \
	CachelinePadded.h \
	CallOnce.h \
	Checksum.h \
	Chrono.h \
	ClockGettimeWrappers.h \
	concurrency/AtomicSharedPtr.h \
	concurrency/CacheLocality.h \
	concurrency/ConcurrentHashMap.h \
	concurrency/CoreCachedSharedPtr.h \
	concurrency/detail/AtomicSharedPtr-detail.h \
	concurrency/detail/ConcurrentHashMap-detail.h \
	concurrency/test/AtomicSharedPtrCounted.h \
	ConcurrentSkipList-inl.h \
	ConcurrentSkipList.h \
	ContainerTraits.h \
	Conv.h \
	CPortability.h \
	CppAttributes.h \
	CpuId.h \
	Demangle.h \
	detail/AtomicHashUtils.h \
	detail/AtomicUnorderedMapUtils.h \
	detail/AtomicUtils.h \
	detail/BitIteratorDetail.h \
	detail/ChecksumDetail.h \
	detail/DiscriminatedPtrDetail.h \
	detail/FileUtilDetail.h \
	detail/FingerprintPolynomial.h \
	detail/Futex.h \
	detail/GroupVarintDetail.h \
	detail/IPAddress.h \
	detail/IPAddressSource.h \
	detail/MallocImpl.h \
	detail/MemoryIdler.h \
	detail/MPMCPipelineDetail.h \
	detail/RangeCommon.h \
	detail/RangeSse42.h \
	detail/Sleeper.h \
	detail/SlowFingerprint.h \
	detail/SocketFastOpen.h \
	detail/StaticSingletonManager.h \
	detail/ThreadLocalDetail.h \
	detail/TryDetail.h \
	detail/TurnSequencer.h \
	detail/UncaughtExceptionCounter.h \
	DiscriminatedPtr.h \
	dynamic-inl.h \
	dynamic.h \
	DynamicConverter.h \
	Enumerate.h \
	EvictingCacheMap.h \
	Exception.h \
	ExceptionString.h \
	ExceptionWrapper-inl.h \
	ExceptionWrapper.h \
	Executor.h \
	Expected.h \
	experimental/AsymmetricMemoryBarrier.h \
	experimental/AutoTimer.h \
	experimental/Bits.h \
	experimental/BitVectorCoding.h \
	experimental/bser/Bser.h \
	experimental/CodingDetail.h \
	experimental/DynamicParser-inl.h \
	experimental/DynamicParser.h \
	experimental/EliasFanoCoding.h \
	experimental/EnvUtil.h \
	experimental/EventCount.h \
	experimental/exception_tracer/ExceptionAbi.h \
	experimental/exception_tracer/ExceptionCounterLib.h \
	experimental/exception_tracer/ExceptionTracer.h \
	experimental/exception_tracer/ExceptionTracerLib.h \
	experimental/exception_tracer/StackTrace.h \
	experimental/ExecutionObserver.h \
	experimental/flat_combining/FlatCombining.h \
	experimental/flat_combining/test/FlatCombiningExamples.h \
	experimental/flat_combining/test/FlatCombiningTestHelpers.h \
	experimental/FlatCombiningPriorityQueue.h \
	experimental/FunctionScheduler.h \
	experimental/FutureDAG.h \
	experimental/hazptr/bench/HazptrBench.h \
	experimental/hazptr/debug.h \
	experimental/hazptr/example/LockFreeLIFO.h \
	experimental/hazptr/example/MWMRSet.h \
	experimental/hazptr/example/SWMRList.h \
	experimental/hazptr/example/WideCAS.h \
	experimental/hazptr/hazptr-impl.h \
	experimental/hazptr/hazptr.h \
	experimental/hazptr/memory_resource.h \
	experimental/hazptr/test/HazptrUse1.h \
	experimental/hazptr/test/HazptrUse2.h \
	experimental/Instructions.h \
	experimental/io/AsyncIO.h \
	experimental/io/FsUtil.h \
	experimental/io/HugePages.h \
	experimental/JemallocNodumpAllocator.h \
	experimental/JSONSchema.h \
	experimental/LockFreeRingBuffer.h \
	experimental/logging/AsyncFileWriter.h \
	experimental/logging/example/lib.h \
	experimental/logging/GlogStyleFormatter.h \
	experimental/logging/ImmediateFileWriter.h \
	experimental/logging/Init.h \
	experimental/logging/LogCategory.h \
	experimental/logging/LogFormatter.h \
	experimental/logging/Logger.h \
	experimental/logging/LoggerDB.h \
	experimental/logging/LogHandler.h \
	experimental/logging/LogLevel.h \
	experimental/logging/LogMessage.h \
	experimental/logging/LogName.h \
	experimental/logging/LogStream.h \
	experimental/logging/LogStreamProcessor.h \
	experimental/logging/LogWriter.h \
	experimental/logging/printf.h \
	experimental/logging/RateLimiter.h \
	experimental/logging/StandardLogHandler.h \
	experimental/logging/test/TestLogHandler.h \
	experimental/logging/test/XlogHeader1.h \
	experimental/logging/test/XlogHeader2.h \
	experimental/logging/xlog.h \
	experimental/NestedCommandLineApp.h \
	experimental/observer/detail/Core.h \
	experimental/observer/detail/GraphCycleDetector.h \
	experimental/observer/detail/Observer-pre.h \
	experimental/observer/detail/ObserverManager.h \
	experimental/observer/Observable-inl.h \
	experimental/observer/Observable.h \
	experimental/observer/Observer-inl.h \
	experimental/observer/Observer.h \
	experimental/observer/SimpleObservable-inl.h \
	experimental/observer/SimpleObservable.h \
	experimental/ProgramOptions.h \
	experimental/RCURefCount.h \
	experimental/RCUUtils.h \
	experimental/ReadMostlySharedPtr.h \
	experimental/Select64.h \
	experimental/StampedPtr.h \
	experimental/StringKeyedCommon.h \
	experimental/StringKeyedMap.h \
	experimental/StringKeyedSet.h \
	experimental/StringKeyedUnorderedMap.h \
	experimental/StringKeyedUnorderedSet.h \
	experimental/symbolizer/Dwarf.h \
	experimental/symbolizer/Elf-inl.h \
	experimental/symbolizer/Elf.h \
	experimental/symbolizer/ElfCache.h \
	experimental/symbolizer/LineReader.h \
	experimental/symbolizer/SignalHandler.h \
	experimental/symbolizer/StackTrace.h \
	experimental/symbolizer/Symbolizer.h \
	experimental/symbolizer/test/SignalHandlerTest.h \
	experimental/test/CodingTestUtils.h \
	experimental/TestUtil.h \
	experimental/ThreadedRepeatingFunctionRunner.h \
	experimental/TLRefCount.h \
	experimental/TupleOps.h \
	FBString.h \
	FBVector.h \
	fibers/AddTasks-inl.h \
	fibers/AddTasks.h \
	fibers/AtomicBatchDispatcher-inl.h \
	fibers/AtomicBatchDispatcher.h \
	fibers/BatchDispatcher.h \
	fibers/Baton-inl.h \
	fibers/Baton.h \
	fibers/BoostContextCompatibility.h \
	fibers/detail/AtomicBatchDispatcher.h \
	fibers/EventBaseLoopController-inl.h \
	fibers/EventBaseLoopController.h \
	fibers/Fiber-inl.h \
	fibers/Fiber.h \
	fibers/FiberManager-inl.h \
	fibers/FiberManager.h \
	fibers/FiberManagerInternal-inl.h \
	fibers/FiberManagerInternal.h \
	fibers/FiberManagerMap.h \
	fibers/ForEach-inl.h \
	fibers/ForEach.h \
	fibers/GenericBaton.h \
	fibers/GuardPageAllocator.h \
	fibers/LoopController.h \
	fibers/Promise-inl.h \
	fibers/Promise.h \
	fibers/Semaphore.h \
	fibers/SimpleLoopController.h \
	fibers/TimedMutex-inl.h \
	fibers/TimedMutex.h \
	fibers/TimeoutController.h \
	fibers/traits.h \
	fibers/WhenN-inl.h \
	fibers/WhenN.h \
	File.h \
	FileUtil.h \
	Fingerprint.h \
	FixedString.h \
	Foreach.h \
	Format-inl.h \
	Format.h \
	FormatArg.h \
	FormatTraits.h \
	Function.h \
	Functional.h \
	futures/Barrier.h \
	futures/detail/Core.h \
	futures/detail/FSM.h \
	futures/detail/Types.h \
	futures/DrivableExecutor.h \
	futures/exercises/Koan.h \
	futures/Future-inl.h \
	futures/Future-pre.h \
	futures/Future.h \
	futures/FutureException.h \
	futures/FutureSplitter.h \
	futures/helpers.h \
	futures/InlineExecutor.h \
	futures/ManualExecutor.h \
	futures/Promise-inl.h \
	futures/Promise.h \
	futures/QueuedImmediateExecutor.h \
	futures/ScheduledExecutor.h \
	futures/SharedPromise-inl.h \
	futures/SharedPromise.h \
	futures/test/TestExecutor.h \
	futures/test/ThenCompileTest.h \
	futures/ThreadWheelTimekeeper.h \
	futures/Timekeeper.h \
	gen/Base-inl.h \
	gen/Base.h \
	gen/Combine-inl.h \
	gen/Combine.h \
	gen/Core-inl.h \
	gen/Core.h \
	gen/File-inl.h \
	gen/File.h \
	gen/Parallel-inl.h \
	gen/Parallel.h \
	gen/ParallelMap-inl.h \
	gen/ParallelMap.h \
	gen/String-inl.h \
	gen/String.h \
	gen/test/Bench.h \
	GlobalThreadPoolList.h \
	GroupVarint.h \
	hash/SpookyHashV1.h \
	hash/SpookyHashV2.h \
	Hash.h \
	Indestructible.h \
	IndexedMemPool.h \
	init/Init.h \
	IntrusiveList.h \
	io/async/AsyncPipe.h \
	io/async/AsyncServerSocket.h \
	io/async/AsyncSignalHandler.h \
	io/async/AsyncSocket.h \
	io/async/AsyncSocketBase.h \
	io/async/AsyncSocketException.h \
	io/async/AsyncSSLSocket.h \
	io/async/AsyncTimeout.h \
	io/async/AsyncTransport.h \
	io/async/AsyncUDPServerSocket.h \
	io/async/AsyncUDPSocket.h \
	io/async/DecoratedAsyncTransportWrapper.h \
	io/async/DelayedDestruction.h \
	io/async/DelayedDestructionBase.h \
	io/async/DestructorCheck.h \
	io/async/EventBase.h \
	io/async/EventBaseLocal.h \
	io/async/EventBaseManager.h \
	io/async/EventBaseThread.h \
	io/async/EventFDWrapper.h \
	io/async/EventHandler.h \
	io/async/EventUtil.h \
	io/async/HHWheelTimer.h \
	io/async/NotificationQueue.h \
	io/async/Request.h \
	io/async/ScopedEventBaseThread.h \
	io/async/ssl/OpenSSLUtils.h \
	io/async/ssl/SSLErrors.h \
	io/async/ssl/TLSDefinitions.h \
	io/async/SSLContext.h \
	io/async/SSLOptions.h \
	io/async/test/AsyncSocketTest.h \
	io/async/test/AsyncSocketTest2.h \
	io/async/test/AsyncSSLSocketTest.h \
	io/async/test/BlockingSocket.h \
	io/async/test/MockAsyncServerSocket.h \
	io/async/test/MockAsyncSocket.h \
	io/async/test/MockAsyncSSLSocket.h \
	io/async/test/MockAsyncTransport.h \
	io/async/test/MockAsyncUDPSocket.h \
	io/async/test/MockTimeoutManager.h \
	io/async/test/ScopedBoundPort.h \
	io/async/test/SocketPair.h \
	io/async/test/TestSSLServer.h \
	io/async/test/TimeUtil.h \
	io/async/test/UndelayedDestruction.h \
	io/async/test/Util.h \
	io/async/TimeoutManager.h \
	io/async/VirtualEventBase.h \
	io/async/WriteChainAsyncTransportWrapper.h \
	io/Compression.h \
	io/Cursor-inl.h \
	io/Cursor.h \
	io/IOBuf.h \
	io/IOBufQueue.h \
	io/RecordIO-inl.h \
	io/RecordIO.h \
	io/ShutdownSocketSet.h \
	io/TypedIOBuf.h \
	IPAddress.h \
	IPAddressException.h \
	IPAddressV4.h \
	IPAddressV6.h \
	Iterator.h \
	json.h \
	Launder.h \
	Lazy.h \
	LifoSem.h \
	Likely.h \
	LockTraits.h \
	LockTraitsBoost.h \
	Logging.h \
	MacAddress.h \
	MallctlHelper.h \
	Malloc.h \
	MapUtil.h \
	Math.h \
	memory/UninitializedMemoryHacks.h \
	Memory.h \
	MemoryMapping.h \
	Merge.h \
	MicroLock.h \
	MicroSpinLock.h \
	MoveWrapper.h \
	MPMCPipeline.h \
	MPMCQueue.h \
	Optional.h \
	Overload.h \
	PackedSyncPtr.h \
	Padded.h \
	Partial.h \
	PicoSpinLock.h \
	portability/Asm.h \
	portability/Atomic.h \
	portability/BitsFunctexcept.h \
	portability/Builtins.h \
	portability/Config.h \
	portability/Constexpr.h \
	portability/Dirent.h \
	portability/Event.h \
	portability/Fcntl.h \
	portability/GFlags.h \
	portability/GMock.h \
	portability/GTest.h \
	portability/IOVec.h \
	portability/Libgen.h \
	portability/Malloc.h \
	portability/Math.h \
	portability/Memory.h \
	portability/OpenSSL.h \
	portability/PThread.h \
	portability/Semaphore.h \
	portability/Sockets.h \
	portability/Stdio.h \
	portability/Stdlib.h \
	portability/String.h \
	portability/SysFile.h \
	portability/Syslog.h \
	portability/SysMembarrier.h \
	portability/SysMman.h \
	portability/SysResource.h \
	portability/SysStat.h \
	portability/SysSyscall.h \
	portability/SysTime.h \
	portability/SysTypes.h \
	portability/SysUio.h \
	portability/Time.h \
	portability/TypeTraits.h \
	portability/Unistd.h \
	portability/Windows.h \
	Portability.h \
	Preprocessor.h \
	PriorityMPMCQueue.h \
	ProducerConsumerQueue.h \
	python/futures.h \
	python/NotificationQueueExecutor.h \
	python/test/simple.h \
	Random-inl.h \
	Random.h \
	Range.h \
	Replaceable.h \
	RWSpinLock.h \
	SafeAssert.h \
	ScopeGuard.h \
	SharedMutex.h \
	Shell.h \
	Singleton-inl.h \
	Singleton.h \
	SingletonThreadLocal.h \
	SingletonVault_c.h \
	small_vector.h \
	SmallLocks.h \
	SocketAddress.h \
	sorted_vector_types.h \
	SparseByteSet.h \
	SpinLock.h \
	ssl/detail/OpenSSLThreading.h \
	ssl/detail/SSLSessionImpl.h \
	ssl/Init.h \
	ssl/OpenSSLCertUtils.h \
	ssl/OpenSSLHash.h \
	ssl/OpenSSLLockTypes.h \
	ssl/OpenSSLPtrTypes.h \
	ssl/OpenSSLVersionFinder.h \
	ssl/SSLSession.h \
	stats/BucketedTimeSeries-defs.h \
	stats/BucketedTimeSeries.h \
	stats/detail/Bucket.h \
	stats/Histogram-defs.h \
	stats/Histogram.h \
	stats/MultiLevelTimeSeries-defs.h \
	stats/MultiLevelTimeSeries.h \
	stats/TimeseriesHistogram-defs.h \
	stats/TimeseriesHistogram.h \
	stop_watch.h \
	String-inl.h \
	String.h \
	Subprocess.h \
	Synchronized.h \
	test/BatonTestHelpers.h \
	test/DeterministicSchedule.h \
	test/FBStringTestBenchmarks.cpp.h \
	test/FBVectorTestBenchmarks.cpp.h \
	test/function_benchmark/benchmark_impl.h \
	test/function_benchmark/test_functions.h \
	test/SingletonTestStructs.h \
	test/SocketAddressTestHelper.h \
	test/SynchronizedTestLib-inl.h \
	test/SynchronizedTestLib.h \
	test/TestUtils.h \
	test/TokenBucketTest.h \
	ThreadCachedArena.h \
	ThreadCachedInt.h \
	ThreadId.h \
	ThreadLocal.h \
	ThreadName.h \
	TimeoutQueue.h \
	TokenBucket.h \
	tracing/StaticTracepoint-ELFx86.h \
	tracing/StaticTracepoint.h \
	Traits.h \
	Try-inl.h \
	Try.h \
	UncaughtExceptions.h \
	Unicode.h \
	Unit.h \
	Uri-inl.h \
	Uri.h \
	Utility.h \
	Varint.h \
	VersionCheck.h

FormatTables.cpp: build/generate_format_tables.py
	$(PYTHON) build/generate_format_tables.py
CLEANFILES += FormatTables.cpp

EscapeTables.cpp: build/generate_escape_tables.py
	$(PYTHON) build/generate_escape_tables.py
CLEANFILES += EscapeTables.cpp

GroupVarintTables.cpp: build/generate_varint_tables.py
	$(PYTHON) build/generate_varint_tables.py
CLEANFILES += GroupVarintTables.cpp

libfollybasesse42_la_SOURCES = \
	detail/Crc32cDetail.cpp \
	detail/ChecksumDetail.cpp \
	detail/RangeSse42.cpp

libfollybase_la_SOURCES = \
	Conv.cpp \
	Demangle.cpp \
	detail/RangeCommon.cpp \
	EscapeTables.cpp \
	Format.cpp \
	FormatArg.cpp \
	FormatTables.cpp \
	MallctlHelper.cpp \
	portability/BitsFunctexcept.cpp \
	String.cpp \
	Unicode.cpp

libfolly_la_SOURCES = \
	Assume.cpp \
	Checksum.cpp \
	ClockGettimeWrappers.cpp \
	concurrency/CacheLocality.cpp \
	detail/IPAddress.cpp \
	dynamic.cpp \
	ExceptionWrapper.cpp \
	Executor.cpp \
	File.cpp \
	FileUtil.cpp \
	FingerprintTables.cpp \
	futures/Barrier.cpp \
	futures/Future.cpp \
	futures/FutureException.cpp \
	futures/ManualExecutor.cpp \
	futures/QueuedImmediateExecutor.cpp \
	futures/ThreadWheelTimekeeper.cpp \
	futures/test/TestExecutor.cpp \
	detail/Futex.cpp \
	detail/StaticSingletonManager.cpp \
	detail/ThreadLocalDetail.cpp \
	hash/SpookyHashV1.cpp \
	hash/SpookyHashV2.cpp \
	GroupVarint.cpp \
	GroupVarintTables.cpp \
	IPAddress.cpp \
	IPAddressV4.cpp \
	IPAddressV6.cpp \
	LifoSem.cpp \
	init/Init.cpp \
	io/Compression.cpp \
	io/Cursor.cpp \
	io/IOBuf.cpp \
	io/IOBufQueue.cpp \
	io/RecordIO.cpp \
	io/ShutdownSocketSet.cpp \
	io/async/AsyncPipe.cpp \
	io/async/AsyncTimeout.cpp \
	io/async/AsyncUDPSocket.cpp \
	io/async/AsyncServerSocket.cpp \
	io/async/AsyncSignalHandler.cpp \
	io/async/AsyncSocket.cpp \
	io/async/AsyncSSLSocket.cpp \
	io/async/EventBase.cpp \
	io/async/EventBaseLocal.cpp \
	io/async/EventBaseManager.cpp \
	io/async/EventBaseThread.cpp \
	io/async/EventHandler.cpp \
	io/async/Request.cpp \
	io/async/SSLContext.cpp \
	io/async/SSLOptions.cpp \
	io/async/ScopedEventBaseThread.cpp \
	io/async/VirtualEventBase.cpp \
	io/async/HHWheelTimer.cpp \
	io/async/TimeoutManager.cpp \
	io/async/test/ScopedBoundPort.cpp \
	io/async/test/SocketPair.cpp \
	io/async/test/TimeUtil.cpp \
	io/async/ssl/OpenSSLUtils.cpp \
	io/async/ssl/SSLErrors.cpp \
	json.cpp \
	detail/MemoryIdler.cpp \
	detail/SocketFastOpen.cpp \
	MacAddress.cpp \
	MemoryMapping.cpp \
	portability/Dirent.cpp \
	portability/Fcntl.cpp \
	portability/Libgen.cpp \
	portability/Malloc.cpp \
	portability/Memory.cpp \
	portability/OpenSSL.cpp \
	portability/PThread.cpp \
	portability/Sockets.cpp \
	portability/Stdio.cpp \
	portability/Stdlib.cpp \
	portability/String.cpp \
	portability/SysFile.cpp \
	portability/SysMembarrier.cpp \
	portability/SysMman.cpp \
	portability/SysResource.cpp \
	portability/SysStat.cpp \
	portability/SysTime.cpp \
	portability/SysUio.cpp \
	portability/Time.cpp \
	portability/Unistd.cpp \
	Random.cpp \
	SafeAssert.cpp \
	ScopeGuard.cpp \
	SharedMutex.cpp \
	Shell.cpp \
	MicroLock.cpp \
	Optional.cpp \
	Singleton.cpp \
	SocketAddress.cpp \
	ssl/Init.cpp \
	ssl/OpenSSLCertUtils.cpp \
	ssl/OpenSSLHash.cpp \
	ssl/detail/OpenSSLThreading.cpp \
	ssl/detail/SSLSessionImpl.cpp \
	stats/BucketedTimeSeries.cpp \
	stats/Histogram.cpp \
	stats/MultiLevelTimeSeries.cpp \
	stats/TimeseriesHistogram.cpp \
	Subprocess.cpp \
	ThreadCachedArena.cpp \
	ThreadName.cpp \
	TimeoutQueue.cpp \
	Try.cpp \
	Uri.cpp \
	Version.cpp \
	experimental/AsymmetricMemoryBarrier.cpp \
	experimental/ThreadedRepeatingFunctionRunner.cpp \
	experimental/bser/Dump.cpp \
	experimental/bser/Load.cpp \
	experimental/DynamicParser.cpp \
	experimental/EnvUtil.cpp \
	experimental/FunctionScheduler.cpp \
	experimental/io/FsUtil.cpp \
	experimental/JemallocNodumpAllocator.cpp \
	experimental/JSONSchema.cpp \
	experimental/NestedCommandLineApp.cpp \
	experimental/observer/detail/Core.cpp \
	experimental/observer/detail/ObserverManager.cpp \
	experimental/ProgramOptions.cpp \
	experimental/Select64.cpp \
	experimental/TestUtil.cpp

if HAVE_LINUX
nobase_follyinclude_HEADERS += \
	experimental/io/HugePages.h
libfolly_la_SOURCES += \
	experimental/io/HugePages.cpp
endif

if !HAVE_WEAK_SYMBOLS
libfollybase_la_SOURCES += detail/MallocImpl.cpp
endif

if HAVE_BOOST_CONTEXT
nobase_follyinclude_HEADERS += \
	fibers/AddTasks.h \
	fibers/AddTasks-inl.h \
	fibers/AtomicBatchDispatcher.h \
	fibers/AtomicBatchDispatcher-inl.h \
	fibers/Baton.h \
	fibers/Baton-inl.h \
	fibers/BatchDispatcher.h \
	fibers/BoostContextCompatibility.h \
	fibers/detail/AtomicBatchDispatcher.h \
	fibers/EventBaseLoopController.h \
	fibers/EventBaseLoopController-inl.h \
	fibers/Fiber.h \
	fibers/Fiber-inl.h \
	fibers/FiberManager.h \
	fibers/FiberManager-inl.h \
	fibers/FiberManagerInternal.h \
	fibers/FiberManagerInternal-inl.h \
	fibers/FiberManagerMap.h \
	fibers/ForEach.h \
	fibers/ForEach-inl.h \
	fibers/GenericBaton.h \
	fibers/GuardPageAllocator.h \
	fibers/LoopController.h \
	fibers/Promise.h \
	fibers/Promise-inl.h \
	fibers/Semaphore.h \
	fibers/SimpleLoopController.h \
	fibers/TimedMutex.h \
	fibers/TimedMutex-inl.h \
	fibers/TimeoutController.h \
	fibers/traits.h \
	fibers/WhenN.h \
	fibers/WhenN-inl.h

libfolly_la_SOURCES += \
	fibers/Baton.cpp \
	fibers/detail/AtomicBatchDispatcher.cpp \
	fibers/Fiber.cpp \
	fibers/FiberManager.cpp \
	fibers/FiberManagerMap.cpp \
	fibers/GuardPageAllocator.cpp \
	fibers/Semaphore.cpp \
	fibers/TimeoutController.cpp
endif

libfollybasesse42_la_LDFLAGS = $(AM_LDFLAGS) -version-info $(LT_VERSION)
libfollybasesse42_la_CXXFLAGS = -msse4.2 -mpclmul

libfollybase_la_LIBADD = libfollybasesse42.la
libfollybase_la_LDFLAGS = $(AM_LDFLAGS) -version-info $(LT_VERSION)

libfolly_la_LIBADD = libfollybase.la
libfolly_la_LDFLAGS = $(AM_LDFLAGS) -version-info $(LT_VERSION) -lssl

FingerprintTables.cpp: generate_fingerprint_tables
	./generate_fingerprint_tables
CLEANFILES += FingerprintTables.cpp

libfollybenchmark_la_SOURCES = Benchmark.cpp
libfollybenchmark_la_LIBADD = libfolly.la
libfollybenchmark_la_LDFLAGS = $(AM_LDFLAGS) -version-info $(LT_VERSION)

# install pkg-config metadata file
pkgconfigdir = $(libdir)/pkgconfig
nodist_pkgconfig_DATA = libfolly.pc
