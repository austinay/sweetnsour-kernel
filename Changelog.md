# **version13** #
  * config: enable data usage stats
  * config: selinux support
  * bcm4325: Clean-up for BCMDONGLEHOST
  * config: revert BCM4325 deep sleep
  * CVE-2013-2094, CVE-2012-4220, CVE-2012-4221, CVE-2012-4222, CVE-2013-2596, CVE-2013-2595
  * Do not ratelimit audit messages. We want to see them all.
  * Enable setting security contexts on rootfs inodes.
  * yaffs: fix getxattr support
  * yaffs: set security attribute at file creation
  * usb:gadget:android: avoid sending extra uevents
  * Add permission checking for binder IPC.
  * config: revert PPP changes
  * Revert "lower swappiness to 0"


# **version12** #
  * set default governor and I/O scheduler to ondemandx and SIO, respectively
  * 3.0.101 kernel
  * FUSE filesystem for KitKat support

# **version11** #
  * acpuclock: undervolt
  * ARM: decompressor: Enable unaligned memory access for v6 and above
  * block: Zen I/O scheduler
  * logger: more ram
  * msm: kgsl: Add CP\_WAIT\_FOR\_IDLE packet before updating timestamp
  * msm: kgsl: Add cache flush for A20x
  * msm: kgsl: Set sysfs max clock for devices with no power scale policy
  * lib: genalloc: Change chunk allocation to vmalloc
  * msm: bam\_dmux: handle system wide low memory conditions
  * msm\_fb: display: Add timeout for waiting on update
  * msm: bam\_dmux: enable disconnect ack feature support by default
  * msm: bam\_dmux: update SSR handling to reflect disconnect ack on by default
  * msm: bam\_dmux: add missing parameter to bam\_dmux\_log() call
  * msm: bam\_dmux: Disable BAM DMUX upon modem timeout
  * msm\_fb: display: Add pre-multiplied alpha support for MDP4
  * msm\_fb: Check for Histogram NULL while queuing work
  * genlock: backport from CAF
  * timed\_gpio: backport from CAF
  * msm: kgsl: Use the right physical addresses in NOMMU mode
  * msm: kgsl: return correct error code for unknown ioctls
  * msm: kgsl: Find a mem\_entry by way of a GPU address and a pagetable base
  * msm: kgsl: Cleanup header file macros
  * msm: kgsl: Do not take spinlock when mapping to IOMMU
  * msm: kgsl: flush cache otherwise memory will be uninitialized
  * msm: kgsl: Add KGSL\_DEV\_ERR\_ONCE helper macro for logging
  * msm: kgsl: Do not dereference pointer before checking against NULL
  * msm: kgsl: Add markers to identify IB sequence start and end
  * msm: kgsl: Allocate physical pages instead of using vmalloc
  * msm: kgsl: Don't call through pwrscale functions when entering SLUMBER
  * msm: kgsl: flush outer cache for alloc\_page() pages
  * msm: kgsl: Resolve conflicts in state changes
  * msm: kgsl: Write the retired timestamp on resume
  * msm: kgsl: Add functions for enabling / disabling a powerscale policy
  * msm: kgsl: Search setstate memory descriptor
  * msm: kgsl: Remove duplicate soptimestamp memory write call
  * msm: kgsl: Use default hardcoded value for CP's ROQ queue size
  * msm: kgsl: Improve the notification timing of idle events
  * msm: kgsl: Properly assign the physical address
  * msm: kgsl: Fix powerscale idle logic
  * msm: kgsl: Make tlb flags common for all MMU types
  * msm: kgsl: Fix when GMEM is saved for A2xx
  * msm: kgsl: fix format of the rbbm read error message
  * msm: kgsl: Pass correct datatype to kgsl\_mmu\_ptpool\_destroy()
  * msm: kgsl: Follow reverse sequence of init procedure during exit
  * msm: kgsl: Only return tlb flush flag if bit is set for given device
  * msm: kgsl: Modify kgsl\_core\_exit to release resources carefully
  * msm: kgsl: Align busy times with the end times of samples
  * makefile: optimizations
  * memcg: let css\_get\_next() rely upon rcu\_read\_lock()
  * kmalloc: Finer grained memory allocation blocks for the ARM11 systems
  * makefile: fix typo
  * 3.0.83 kernel

# **version10** #
  * mcs6000: update
  * Start wlan after deep-sleep
  * bcm4325: Move sources into main folder
  * bcm4325: Delete unnecessary files
  * qdsp5: Incall recording pcm driver
  * Qualcomm ROW scheduler
  * block: row: fix compatibility with 3.0 Kernel code
  * config: add row scheduler, set performance as default, default TS driver
  * deadline: Allow 0ms deadline latency, increase the read speed
  * block: row: hardcode values research by the community
  * config: turn off module versioning
  * 3.0.81 kernel

# **version9d** #
  * Forward port bluetooth drivers from jb\_mr1\_chocolate
  * Revert "Major changes to RWSEM algorithm"
  * config: enable netfilter owner feature for orbot
  * 3.0.78 kernel

# **version9c** #
  * 3.0.73 kernel
  * config: enable fast charge, support for triple buffer

# **version9b** #
  * increased VM dirty writeback time to 15 seconds
  * many changes to config
  * increase min readahead
  * implement USB fast charge from chad0989

# **version9a** #
  * Add dynamic writeback feature from 3.1
  * Revert "rwsem: steal writing sem for better performance"
  * Revert "rwsem-spinlock: let rwsem write lock stealable"
  * Major changes to RWSEM algorithm
  * config: enable CFS-related options
  * config: enable CONFIG\_CPU\_FREQ\_STAT, smartassv2 as default
  * config: revert previous change

# **version9** #
  * config: tweaks
  * increase readahead to 2048
  * many P350-related commits
  * config: no harm in enabling PPP options
  * config: fix RAM readings
  * config: set CFS as default, enable CONFIG\_SCHED\_AUTOGROUP
  * 3.0.72 kernel

# **version8c** #
  * makefile: arm6 optimizations from fserve
  * config: TESTING (battery)
  * use Der Caveman's touchscreen driver

# **version8b** #
  * we can take the punishment of higher gpu bus clock
  * Enable deep sleep on BCM4325
  * net: fix bcm4325

# **version8a** #
  * LGE\_POWER\_ON\_STATUS\_PATCH
  * mm: optimize Kernel Samepage Merging(KSM)
  * kernel:sched: LOAD\_FREQ (4\*HZ+61) avoids loadavg Moire
  * vfp: use hard float
  * lib/checksum.c: optimize do\_csum a bit
  * rwsem-spinlock: let rwsem write lock stealable
  * Enable deep sleep on BCM4325
  * config: another attempt at PPTP

# **version8** #
  * 3.0.68 kernel
  * acpuclock: include 710 mhz
  * fix permission issue which prevents "active tasks" shown in
  * config: enable data limit
  * config: PPTP

# **version7d** #
  * LGE\_POWER\_ON\_STATUS\_PATCH
  * Forward port bluetooth drivers from jb\_mr1\_chocolate
  * Revert "Revert "we can take the punishment of higher gpu bus clock""
  * Revert "Revert "on request, make this global for all lge devices""
  * Revert "rwsem-spinlock: let rwsem write lock stealable"
  * Revert "rwsem: steal writing sem for better performance"
  * config: enable netfilter owner feature for orbot
  * config: enable CFS-related options
  * config: enable triple buffer

# **version7c** #
  * mm: optimize Kernel Samepage Merging(KSM)
  * kernel:sched: LOAD\_FREQ (4\*HZ+61) avoids loadavg Moire
  * vfp: use hard float
  * lib/checksum.c: optimize do\_csum a bit
  * rwsem-spinlock: let rwsem write lock stealable
  * we can take the punishment of higher gpu bus clock
  * Enable deep sleep on BCM4325
  * net: fix bcm4325
  * makefile: arm6 optimizations from fserve

# **version7b** #
  * block: tweak SIO scheduler

# **version7a** #
  * Revert "LCD: Fix deadlock on displaying to panel"
  * Revert "msm: cpufreq: Release cpumask\_var\_t on all cases"
  * Revert "msm: audio: qdsp5: Fix for logical errors in qdsp5"
  * Revert "msm: qdsp5: Fix logging adsp messages for 32-bit address"
  * Revert "msm: smd: Fix race condition while processing SMSM callback"
  * Revert "msm: smsm: Cache Flush on SMSM\_RESET"
  * Revert "msm: smd\_pkt: fix wake lock locking race condition"
  * Revert "msm: smd\_pkt: Fix wakelock concurrency issue"
  * Revert "msm: gic: Remove manual GIC programming for PPI trigger type"
  * Revert "cpufreq: Add cpu utilization statistics to aid decisions made by userspace"
  * Revert "cpufreq: Fix sysfs deadlock with concurrent hotplug/frequency switch"
  * Revert "This is a combination of 13 commits."
  * Revert "This is a combination of 29 commits."
  * Revert "iommu: Fix flags passed to iommu map functions."

# **version7** #
  * msm: cpufreq: Release cpumask\_var\_t on all cases
  * msm: audio: qdsp5: Fix for logical errors in qdsp5
  * msm: qdsp5: Fix logging adsp messages for 32-bit address
  * msm: smd: Fix race condition while processing SMSM callback
  * msm: smsm: Cache Flush on SMSM\_RESET
  * msm: smd\_pkt: fix wake lock locking race condition
  * msm: smd\_pkt: Fix wakelock concurrency issue
  * msm: gic: Remove manual GIC programming for PPI trigger type
  * cpufreq: Add cpu utilization statistics to aid decisions made by userspace
  * cpufreq: Fix sysfs deadlock with concurrent hotplug/frequency switch
  * iommu: Fix flags passed to iommu map functions.
  * proc: clean up and fix /proc/pid/mem handling
  * WIFI PM = FAST
  * config: disable event debugging
  * Implement OC properly for msm7x27 and msm7x27T

# **version6** #
  * cpufreq: adjust conservative governor to save battery
  * cpufreq: add MIN\_TICKS and SAMPLING\_LATENCY\_MULTIPLIER
  * PM / Sleep: Do not check wakeup too often in try\_to\_freeze\_tasks()
  * mm: swaptoken only when swap full
  * mm: drop swap cache aggressively
  * staging: android: lowmemorykiller: Don't count reserved free memory
  * mm: background scan
  * msm: memory: Use standard cache routines
  * mmc: Make sure host is disabled on suspend
  * genlock: don't spam our log. Thx.
  * LCD: Fix deadlock on displaying to panel
  * LCD: Enable dithering on mdp dma operation
  * Cleanup and include some LG things from 2.6
  * rwsem: steal writing sem for better performance
  * config: enable options for PPTP
  * reintroduce thachtunganh's optimized touchscreen driver (special thanks to DJNoXD for helping me fix a compilation issue)
  * config: enable TUN

# **version5c** #
  * enable ZRAM
  * attempt to enable OTG
  * attempt to fix failure of WIFI to connect to networks

# **version5b** #
  * BFS 413
  * Build event debugger as module (to prevent log spam) (hephappy)
  * TWEAK: set rr\_interval to 2 for BFS kernel

# **version5a** #
  * acpuclock: OC stability fixes (androidarmv6)
  * p500: Fix proximity sensor (thanks cyrix.vs)
  * Repair the Novatek driver (androidarmv6)

# **version5** #
  * 3.0.8 kernel
  * use DerCaveman TS driver for now
  * fix wlan wakeup after sleep (androidarmv6)

# **--------------------------------------------------------** #

# **versionFINAL** #
  * acpuclock: undervolt
  * ARM: decompressor: Enable unaligned memory access for v6 and above
  * logger: more ram
  * msm: kgsl: Add CP\_WAIT\_FOR\_IDLE packet before updating timestamp
  * msm: kgsl: Add cache flush for A20x
  * msm: kgsl: Set sysfs max clock for devices with no power scale policy
  * lib: genalloc: Change chunk allocation to vmalloc
  * timed\_gpio: backport from CAF
  * msm: kgsl: Use the right physical addresses in NOMMU mode
  * msm: kgsl: return correct error code for unknown ioctls
  * msm: kgsl: Cleanup header file macros
  * msm: kgsl: Do not take spinlock when mapping to IOMMU
  * msm: kgsl: flush cache otherwise memory will be uninitialized
  * msm: kgsl: Add KGSL\_DEV\_ERR\_ONCE helper macro for logging
  * msm: kgsl: Do not dereference pointer before checking against NULL
  * msm: kgsl: flush outer cache for alloc\_page() pages
  * msm: kgsl: Write the retired timestamp on resume
  * msm: kgsl: Remove duplicate soptimestamp memory write call
  * msm: kgsl: Use default hardcoded value for CP's ROQ queue size
  * msm: kgsl: Improve the notification timing of idle events
  * msm: kgsl: Properly assign the physical address
  * msm: kgsl: Fix when GMEM is saved for A2xx
  * msm: kgsl: fix format of the rbbm read error message
  * msm: kgsl: Pass correct datatype to kgsl\_mmu\_ptpool\_destroy()
  * msm: kgsl: Follow reverse sequence of init procedure during exit
  * msm: kgsl: Modify kgsl\_core\_exit to release resources carefully
  * msm: kgsl: Align busy times with the end times of samples
  * makefile: optimizations
  * memcg: let css\_get\_next() rely upon rcu\_read\_lock()
  * kmalloc: Finer grained memory allocation blocks for the ARM11 systems

# **version4e** #
  * config: enable netfilter owner feature for orbot

# **version4d** #
  * config: battery tweaks

# **version4c** #
  * mm: optimize Kernel Samepage Merging(KSM)
  * kernel:sched: LOAD\_FREQ (4\*HZ+61) avoids loadavg Moire
  * vfp: use hard float
  * lib/checksum.c: optimize do\_csum a bit
  * rwsem-spinlock: let rwsem write lock stealable

# **version4b** #
  * TWEAK: set rr\_interval to 2 for BFS kernel
  * cpufreq: adjust conservative governor to save battery
  * cpufreq: add MIN\_TICKS and SAMPLING\_LATENCY\_MULTIPLIER
  * mm: swaptoken only when swap full
  * mm: drop swap cache aggressively
  * staging: android: lowmemorykiller: Don't count reserved free memory
  * mm: background scan
  * msm: memory: Use standard cache routines
  * mmc: Make sure host is disabled on suspend
  * config: enable options for PPTP

# **version4a** #
  * test DerCaveman touchscreen driver on 2.6.35.14

# **version4** #
  * use optimized mcs6000 touchscreen driver
  * enablel RNDIS for USB tethering
  * use CodeSourcery toolchain
  * net sched: fix some kernel memory leaks
  * net/ipv4: Eliminate kstrdup memory leak
  * Remove BUGVERBOSE - francofrancisco
  * shmem: reduce pagefault lock contention
  * posix-timers: RCU conversion
  * percpu: zero memory more efficiently in mm/percpu.c::pcpu\_mem\_alloc()

# **version3a** #
  * return to stock voltages

# **version3** #
  * attempt to fix axis inversion
  * memory patches
```
 * mm: ashmem: fix deadlock when system is low on memory
 * sched: Fix struct autogroup memory leak
 * staging: android: lowmemorykiller: Change default debug_level to 1
 * fix memory leaks from the wifi drivers (franciscofranco)
 * msm: Increase DMA consistent memory zone to 14MB
```
  * init: calibrate: Backported from 3.0 kernel.
  * The new jhash implementation
  * Update kernel config
  * block: tweaked deadline for better performance
  * msm: kgsl: Update pagetable on context destruction for A20x
  * msm: kgsl: Increase REG\_RBBM\_CNTL value to 0xFFFF for A200
  * Fast Sleep, wake lock timer change. (wistilt2)
  * introduce frandom module
  * sched: don't call task\_group() many times in set\_task\_rq()
  * SmartassV2 is back
  * Squashed ipv6 patches

# **version2** #
  * add axis inversion workaround and pressure sensitivity
  * enable AXI OC
  * CPUIDLE driver from 3.7
  * staging: framebuffer port from 3.0.8
  * mmc: use really long write timeout to deal with crappy cards
  * New battery driver courtesy of thachtunganh
  * reclaim RAM from loggers, optimized kernel
  * add more PMEM
  * Removed unnecessary crap: saves battery life (Rashed97)
  * enable TINY RCU

# **version1** #

  * performance patches
```
 *decreased vfs_cache_pressure
 *set slub_max_order to 0
 *tweak SIO scheduler
 *tweak dirty_background_ratio, vm_dirty_ratio
 *lib: Improve the performance of memcpy and memmove of the general version (arco)
 *patched vm_max_readahead
 *sched: disable GENTLE_FAIR_SLEEPERS
 *tweak deadline I/O scheduler
 *lower swappiness to 0 (low latency)
 *optimize xz wrapper to speed up boot time (sar castillo)
 *tweak conservative governor
 *mm: writeback: disable the writeback function while the screen is on
 *CFS tweaks
 *use O3 optimization
 *use franciscofranco's touchscreen driver
 *implement BFS 404
```
  * power management patches
```
 *patches from thachtunganh
 *kernel: Prevent unnecessary rfkill event generation (Vitaly Wool)
```
  * Google Snappy compression for ZRAM
  * add SLQB memory allocator
  * add Stochastic Fair Blue network scheduler
  * attempt to show WIFI networks with low signal
  * Hack for CRT animations fix (Rashed97)
  * Fix mdp4\_overlay for MDPI devices (Rashed97)
  * fix lowmemorykiller.c: memory compaction is never invoked
  * WIFI PM = FAST (thachtunganh)
  * Proportional Rate Reduction for TCP
  * update from 2.6.35.10 to 2.6.35.14
  * increase vibration
  * added optimized CRC32 algorithm (Ezekeel)