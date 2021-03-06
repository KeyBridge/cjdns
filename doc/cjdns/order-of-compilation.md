Here is the order of compilation on  my Linux box (3.13.0-43-generic #72-Ubuntu SMP x86_64) of `*.c` files when `./do` spawns `gcc` using '`-c`', '`-S`' or '`-E`':

The top-most files were compiled first, and has the least number of dependencies. This listing includes the compilation of `cnacl` and `libuv` libraries included in the source tree.

1. `cjdns/node_build/dependencies/cnacl/randombytes/devurandom.c`
1. `cjdns/node_build/dependencies/cnacl/okcompilers/abiname_xcompile.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_hashblocks/sha512/inplace/blocks.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_scalarmult/curve25519/donna_c64/base.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_scalarmult/curve25519/donna_c64/smult.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_verify/16/ref/verify.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_hash/sha512/ref/hash.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_box/curve25519xsalsa20poly1305/ref/after.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_box/curve25519xsalsa20poly1305/ref/before.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_box/curve25519xsalsa20poly1305/ref/box.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_box/curve25519xsalsa20poly1305/ref/keypair.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_onetimeauth/poly1305/amd64/verify.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_stream/xsalsa20/ref/stream.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_stream/xsalsa20/ref/xor.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_core/salsa208/ref/core.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_stream/aes128ctr/core2/stream.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_stream/aes128ctr/core2/xor.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_hashblocks/sha256/ref/blocks.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_core/hsalsa20/ref/core.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_verify/32/ref/verify.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_core/salsa2012/ref/core.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_hash/sha256/ref/hash.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_core/salsa20/ref/core.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_auth/hmacsha256/ref/hmac.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_auth/hmacsha256/ref/verify.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_secretbox/xsalsa20poly1305/ref/box.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_auth/hmacsha512256/ref/hmac.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_auth/hmacsha512256/ref/verify.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_0.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_1.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_add.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_cmov.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_copy.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_frombytes.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_invert.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_isnegative.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_isnonzero.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_mul.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_neg.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_pow22523.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_sq.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_sq2.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_sub.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/fe_tobytes.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_add.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_double_scalarmult.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_frombytes.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_madd.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_msub.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p1p1_to_p2.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p1p1_to_p3.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p2_0.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p2_dbl.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p3_0.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p3_dbl.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p3_to_cached.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p3_to_p2.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_p3_tobytes.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_precomp_0.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_scalarmult_base.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_sub.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/ge_tobytes.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/keypair.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/open.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/sc_muladd.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/sc_reduce.c`
1. `cjdns/node_build/dependencies/cnacl/crypto_sign/ed25519/ref10/sign.c`
1. `cjdns/node_build/dependencies/libuv/src/fs-poll.c`
1. `cjdns/node_build/dependencies/libuv/src/inet.c`
1. `cjdns/node_build/dependencies/libuv/src/version.c`
1. `cjdns/node_build/dependencies/libuv/src/uv-common.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/async.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/core.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/dl.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/fs.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/getaddrinfo.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/loop.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/loop-watcher.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/pipe.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/poll.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/process.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/signal.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/stream.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/tcp.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/thread.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/threadpool.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/timer.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/tty.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/udp.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/proctitle.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/linux-core.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/linux-inotify.c`
1. `cjdns/node_build/dependencies/libuv/src/unix/linux-syscalls.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-async.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-fs-stat.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-async-pummel.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-getaddrinfo.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-loop-count.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-million-async.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-million-timers.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-multi-accept.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-ping-pongs.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-pound.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-pump.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-sizes.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-spawn.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-thread.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-tcp-write-batch.c`
1. `cjdns/node_build/dependencies/libuv/test/benchmark-udp-pummel.c`
1. `cjdns/node_build/dependencies/libuv/test/dns-server.c`
1. `cjdns/node_build/dependencies/libuv/test/echo-server.c`
1. `cjdns/node_build/dependencies/libuv/test/blackhole-server.c`
1. `cjdns/node_build/dependencies/libuv/test/run-benchmarks.c`
1. `cjdns/node_build/dependencies/libuv/test/runner.c`
1. `cjdns/node_build/dependencies/libuv/test/runner-unix.c`
1. `cjdns/node_build/dependencies/libuv/test/blackhole-server.c`
1. `cjdns/node_build/dependencies/libuv/test/echo-server.c`
1. `cjdns/node_build/dependencies/libuv/test/run-tests.c`
1. `cjdns/node_build/dependencies/libuv/test/test-get-loadavg.c`
1. `cjdns/node_build/dependencies/libuv/test/runner.c`
1. `cjdns/node_build/dependencies/libuv/test/test-active.c`
1. `cjdns/node_build/dependencies/libuv/test/test-async.c`
1. `cjdns/node_build/dependencies/libuv/test/test-async-null-cb.c`
1. `cjdns/node_build/dependencies/libuv/test/test-callback-stack.c`
1. `cjdns/node_build/dependencies/libuv/test/test-callback-order.c`
1. `cjdns/node_build/dependencies/libuv/test/test-close-fd.c`
1. `cjdns/node_build/dependencies/libuv/test/test-close-order.c`
1. `cjdns/node_build/dependencies/libuv/test/test-connection-fail.c`
1. `cjdns/node_build/dependencies/libuv/test/test-cwd-and-chdir.c`
1. `cjdns/node_build/dependencies/libuv/test/test-delayed-accept.c`
1. `cjdns/node_build/dependencies/libuv/test/test-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-embed.c`
1. `cjdns/node_build/dependencies/libuv/test/test-emfile.c`
1. `cjdns/node_build/dependencies/libuv/test/test-fail-always.c`
1. `cjdns/node_build/dependencies/libuv/test/test-fs.c`
1. `cjdns/node_build/dependencies/libuv/test/test-fs-event.c`
1. `cjdns/node_build/dependencies/libuv/test/test-get-currentexe.c`
1. `cjdns/node_build/dependencies/libuv/test/test-get-memory.c`
1. `cjdns/node_build/dependencies/libuv/test/test-getaddrinfo.c`
1. `cjdns/node_build/dependencies/libuv/test/test-getsockname.c`
1. `cjdns/node_build/dependencies/libuv/test/test-hrtime.c`
1. `cjdns/node_build/dependencies/libuv/test/test-idle.c`
1. `cjdns/node_build/dependencies/libuv/test/test-iocp.c`
1. `cjdns/node_build/dependencies/libuv/test/test-ipc.c`
1. `cjdns/node_build/dependencies/libuv/test/test-ipc-send-recv.c`
1. `cjdns/node_build/dependencies/libuv/test/test-loop-handles.c`
1. `cjdns/node_build/dependencies/libuv/test/test-loop-alive.c`
1. `cjdns/node_build/dependencies/libuv/test/test-loop-stop.c`
1. `cjdns/node_build/dependencies/libuv/test/test-walk-handles.c`
1. `cjdns/node_build/dependencies/libuv/test/test-loop-time.c`
1. `cjdns/node_build/dependencies/libuv/test/test-watcher-cross-stop.c`
1. `cjdns/node_build/dependencies/libuv/test/test-multiple-listen.c`
1. `cjdns/node_build/dependencies/libuv/test/test-osx-select.c`
1. `cjdns/node_build/dependencies/libuv/test/test-pass-always.c`
1. `cjdns/node_build/dependencies/libuv/test/test-ping-pong.c`
1. `cjdns/node_build/dependencies/libuv/test/test-pipe-bind-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-pipe-connect-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-pipe-server-close.c`
1. `cjdns/node_build/dependencies/libuv/test/test-platform-output.c`
1. `cjdns/node_build/dependencies/libuv/test/test-poll.c`
1. `cjdns/node_build/dependencies/libuv/test/test-poll-close.c`
1. `cjdns/node_build/dependencies/libuv/test/test-process-title.c`
1. `cjdns/node_build/dependencies/libuv/test/test-ref.c`
1. `cjdns/node_build/dependencies/libuv/test/test-run-nowait.c`
1. `cjdns/node_build/dependencies/libuv/test/test-run-once.c`
1. `cjdns/node_build/dependencies/libuv/test/test-semaphore.c`
1. `cjdns/node_build/dependencies/libuv/test/test-shutdown-close.c`
1. `cjdns/node_build/dependencies/libuv/test/test-shutdown-eof.c`
1. `cjdns/node_build/dependencies/libuv/test/test-signal.c`
1. `cjdns/node_build/dependencies/libuv/test/test-spawn.c`
1. `cjdns/node_build/dependencies/libuv/test/test-signal-multiple-loops.c`
1. `cjdns/node_build/dependencies/libuv/test/test-fs-poll.c`
1. `cjdns/node_build/dependencies/libuv/test/test-stdio-over-pipes.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-bind-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-bind6-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-close.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-close-accept.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-close-while-connecting.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-connect-error-after-write.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-shutdown-after-write.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-flags.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-connect-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-connect-timeout.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-connect6-error.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-open.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-write-to-half-open-connection.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-writealot.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-try-write.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-unexpected-read.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tcp-read-stop.c`
1. `cjdns/node_build/dependencies/libuv/test/test-threadpool.c`
1. `cjdns/node_build/dependencies/libuv/test/test-threadpool-cancel.c`
1. `cjdns/node_build/dependencies/libuv/test/test-mutexes.c`
1. `cjdns/node_build/dependencies/libuv/test/test-thread.c`
1. `cjdns/node_build/dependencies/libuv/test/test-barrier.c`
1. `cjdns/node_build/dependencies/libuv/test/test-condvar.c`
1. `cjdns/node_build/dependencies/libuv/test/test-timer-again.c`
1. `cjdns/node_build/dependencies/libuv/test/test-timer-from-check.c`
1. `cjdns/node_build/dependencies/libuv/test/test-timer.c`
1. `cjdns/node_build/dependencies/libuv/test/test-tty.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-dgram-too-big.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-open.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-ipv6.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-options.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-send-and-recv.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-multicast-join.c`
1. `cjdns/node_build/dependencies/libuv/test/test-dlerror.c`
1. `cjdns/node_build/dependencies/libuv/test/test-udp-multicast-ttl.c`
1. `cjdns/node_build/dependencies/libuv/test/test-ip4-addr.c`
1. `cjdns/node_build/dependencies/libuv/test/test-ip6-addr.c`
1. `cjdns/node_build/dependencies/libuv/test/runner-unix.c`
1. `cjdns/admin/angel/cjdroute2.c`
1. `cjdns/contrib/c/publictoip6.c`
1. `cjdns/contrib/c/privatetopublic.c`
1. `cjdns/contrib/c/sybilsim.c`
1. `cjdns/contrib/c/makekeys.c`
1. `cjdns/crypto/random/randombytes.c`
1. `cjdns/test/testcjdroute.c`
1. `cjdns/util/platform/Sockaddr.c`
1. `cjdns/util/Hex.c`
1. `cjdns/crypto/Key.c`
1. `cjdns/benc/String.c`
1. `cjdns/util/CString.c`
1. `cjdns/memory/Allocator.c`
1. `cjdns/util/Assert.c`
1. `cjdns/dht/Address.c`
1. `cjdns/crypto/AddressCalc.c`
1. `cjdns/memory/MallocAllocator.c`
1. `cjdns/crypto/random/Random.c`
1. `cjdns/crypto/random/seed/RandomSeed.c`
1. `cjdns/util/log/Log.c`
1. `cjdns/exception/Except.c`
1. `cjdns/util/log/WriterLog.c`
1. `cjdns/util/Security.c`
1. `cjdns/util/events/libuv/Process.c`
1. `cjdns/util/events/libuv/Pipe.c`
1. `cjdns/util/SysInfo.c`
1. `cjdns/util/ArchInfo.c`
1. `cjdns/net/SwitchPinger_admin.c`
1. `cjdns/benc/serialization/standard/BencMessageWriter.c`
1. `cjdns/benc/serialization/standard/BencMessageReader.c`
1. `cjdns/benc/serialization/json/JsonBencSerializer.c`
1. `cjdns/io/FileWriter.c`
1. `cjdns/io/FileReader.c`
1. `cjdns/interface/UDPInterface_admin.c`
1. `cjdns/interface/InterfaceController.c`
1. `cjdns/net/SwitchPinger.c`
1. `cjdns/dht/dhtcore/RouterModule_admin.c`
1. `cjdns/dht/dhtcore/RouterModule.c`
1. `cjdns/dht/dhtcore/NodeStore.c`
1. `cjdns/dht/SerializationModule.c`
1. `cjdns/dht/ReplyModule.c`
1. `cjdns/crypto/CryptoAuth_benchmark.c`
1. `cjdns/admin/Configurator.c`
1. `cjdns/admin/AuthorizedPasswords.c`
1. `cjdns/crypto/CryptoAuth.c`
1. `cjdns/admin/angel/Core.c`
1. `cjdns/net/Ducttape.c`
1. `cjdns/util/version/Version.c`
1. `cjdns/tunnel/IpTunnel.c`
1. `cjdns/admin/angel/Hermes.c`
1. `cjdns/switch/SwitchCore.c`
1. `cjdns/dht/dhtcore/RumorMill.c`
1. `cjdns/dht/dhtcore/Router.c`
1. `cjdns/dht/dhtcore/Node.c`
1. `cjdns/switch/EncodingScheme.c`
1. `cjdns/benc/List.c`
1. `cjdns/dht/DHTModuleRegistry.c`
1. `cjdns/admin/angel/AngelInit.c`
1. `cjdns/admin/angel/InterfaceWaiter.c`
1. `cjdns/admin/AdminClient.c`
1. `cjdns/admin/Admin.c`
1. `cjdns/util/events/libuv/EventBase.c`
1. `cjdns/benc/Dict.c`
1. `cjdns/io/ArrayWriter.c`
1. `cjdns/util/events/libuv/Timeout.c`
1. `cjdns/crypto/random/libuv/LibuvEntropyProvider.c`
1. `cjdns/util/log/FileWriterLog.c`
1. `cjdns/io/ArrayReader.c`
1. `cjdns/./interface/tuntap/windows/test/TAPInterface_root_test.c`
1. `cjdns/./interface/tuntap/windows/test/TAPDevice_root_test.c`
1. `cjdns/./util/platform/test/Sockaddr_test.c`
1. `cjdns/./interface/tuntap/test/TUNInterface_ipv6_root_test.c`
1. `cjdns/./interface/tuntap/test/TUNInterface_ipv4_root_test.c`
1. `cjdns/./interface/tuntap/test/TAPWrapper_root_test.c`
1. `cjdns/./dht/dhtcore/test/VersionList_test.c`
1. `cjdns/./crypto/random/test/Random_test.c`
1. `cjdns/./util/test/UniqueName_test.c`
1. `cjdns/./util/test/Seccomp_test.c`
1. `cjdns/./util/test/Process_test.c`
1. `cjdns/./util/test/Map_test.c`
1. `cjdns/./util/test/Identity_test.c`
1. `cjdns/./util/test/Hex_test.c`
1. `cjdns/./util/test/Endian_test.c`
1. `cjdns/./util/test/Checksum_test.c`
1. `cjdns/./util/test/Bits_test.c`
1. `cjdns/./util/test/Base32_test.c`
1. `cjdns/./util/test/Base10_test.c`
1. `cjdns/./util/test/AverageRoller_test.c`
1. `cjdns/./util/test/ArchInfo_test.c`
1. `cjdns/./util/test/AddrTools_test.c`
1. `cjdns/./tunnel/test/IpTunnel_test.c`
1. `cjdns/./switch/test/PenaltyFloat_test.c`
1. `cjdns/./switch/test/NumberCompress_test.c`
1. `cjdns/./switch/test/LabelSplicer_test.c`
1. `cjdns/./switch/test/EncodingScheme_test.c`
1. `cjdns/./memory/test/Allocator_test.c`
1. `cjdns/./io/test/FileReader_test.c`
1. `cjdns/./interface/test/UDPInterface_test.c`
1. `cjdns/./interface/test/UDPInterface_communication_test.c`
1. `cjdns/./interface/test/MultiInterface_test.c`
1. `cjdns/./interface/test/InterfaceController_test.c`
1. `cjdns/./interface/test/InterfaceController_multiIface_test.c`
1. `cjdns/./interface/test/FramingInterface_test.c`
1. `cjdns/./interface/test/FramingInterface_fuzz_test.c`
1. `cjdns/./dht/test/DHTModules_handleOutgoing_test.c`
1. `cjdns/./dht/test/DHTModules_handleIncoming_test.c`
1. `cjdns/./crypto/test/ReplayProtector_test.c`
1. `cjdns/./crypto/test/CryptoAuth_unit_test.c`
1. `cjdns/./crypto/test/CryptoAuth_test.c`
1. `cjdns/./crypto/test/CryptoAuth_async_test.c`
1. `cjdns/./admin/test/Admin_test.c`
1. `cjdns/./test/threeNodes_test.c`
1. `cjdns/./test/printIp_test.c`
1. `cjdns/./test/cjdroute_routerPing_test.c`
1. `cjdns/./test/cjdroute_injection_test.c`
1. `cjdns/./test/CryptoAddress_test.c`
1. `cjdns/util/events/libuv/Time.c`
1. `cjdns/crypto/random/seed/SystemRandomSeed.c`
1. `cjdns/util/Seccomp.c`
1. `cjdns/util/Base10.c`
1. `cjdns/interface/UDPInterface.c`
1. `cjdns/dht/dhtcore/ReplySerializer.c`
1. `cjdns/util/Pinger.c`
1. `cjdns/util/AverageRoller.c`
1. `cjdns/dht/dhtcore/VersionList.c`
1. `cjdns/util/events/libuv/Event.c`
1. `cjdns/interface/SessionManager_admin.c`
1. `cjdns/interface/SessionManager.c`
1. `cjdns/util/Security_admin.c`
1. `cjdns/util/platform/netdev/NetDev.c`
1. `cjdns/util/log/IndirectLog.c`
1. `cjdns/tunnel/IpTunnel_admin.c`
1. `cjdns/memory/Allocator_admin.c`
1. `cjdns/interface/addressable/PacketHeaderToUDPAddrInterface.c`
1. `cjdns/interface/DNSServer.c`
1. `cjdns/interface/RainflyClient_admin.c`
1. `cjdns/interface/RainflyClient.c`
1. `cjdns/interface/FramingInterface.c`
1. `cjdns/interface/InterfaceController_admin.c`
1. `cjdns/interface/InterfaceConnector.c`
1. `cjdns/interface/tuntap/TUNInterface_linux.c`
1. `cjdns/interface/ETHInterface_admin.c`
1. `cjdns/util/events/libuv/UDPAddrInterface.c`
1. `cjdns/dht/dhtcore/Janitor.c`
1. `cjdns/dht/dhtcore/NodeStore_admin.c`
1. `cjdns/dht/dhtcore/SearchRunner_admin.c`
1. `cjdns/dht/dhtcore/SearchRunner.c`
1. `cjdns/dht/EncodingSchemeModule.c`
1. `cjdns/admin/angel/Angel.c`
1. `cjdns/admin/AdminLog.c`
1. `cjdns/switch/Penalty.c`
1. `cjdns/benc/serialization/cloner/Cloner.c`
1. `cjdns/interface/tuntap/test/TUNTools.c`
1. `cjdns/admin/testframework/AdminTestFramework.c`
1. `cjdns/interface/tuntap/TAPWrapper.c`
1. `cjdns/interface/tuntap/NDPServer.c`
1. `cjdns/crypto/random/test/DeterminentRandomSeed.c`
1. `cjdns/util/Order.c`
1. `cjdns/test/TestFramework.c`
1. `cjdns/util/platform/Socket.c`
1. `cjdns/interface/MultiInterface.c`
1. `cjdns/crypto/random/seed/ProcSysKernelRandomUuidRandomSeed.c`
1. `cjdns/interface/MultiInterface.c`
1. `cjdns/crypto/random/seed/ProcSysKernelRandomUuidRandomSeed.c`
1. `cjdns/crypto/random/seed/LinuxRandomUuidSysctlRandomSeed.c`
1. `cjdns/crypto/random/seed/DevUrandomRandomSeed.c`
1. `cjdns/util/platform/netdev/NetPlatform_linux.c`
1. `cjdns/memory/BufferAllocator.c`
1. `cjdns/interface/ETHInterface_linux.c`
1. `cjdns/dht/dhtcore/SearchStore.c`
1. `cjdns/interface/addressable/AddrInterfaceAdapter.c`
