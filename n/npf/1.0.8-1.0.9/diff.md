# Comparing `tmp/npf-1.0.8.tar.gz` & `tmp/npf-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/npf-1.0.8.tar", last modified: Mon Dec 14 10:50:43 2020, max compression
+gzip compressed data, was "dist/npf-1.0.9.tar", last modified: Tue Dec 22 15:53:21 2020, max compression
```

## Comparing `npf-1.0.8.tar` & `npf-1.0.9.tar`

### file list

```diff
@@ -1,144 +1,145 @@
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/
--rwxr-xr-x   0 tom       (1001) nslab     (1000)     7584 2020-12-04 11:50:41.000000 npf-1.0.8/npf_compare.py
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/
--rw-r--r--   0 tom       (1001) nslab     (1000)     3279 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)      100 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)       47 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/top_level.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)      177 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/requires.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)        1 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)    19853 2020-12-14 10:50:43.000000 npf-1.0.8/npf.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1001) nslab     (1000)       42 2020-12-03 13:57:41.000000 npf-1.0.8/MANIFEST.in
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/modules/
--rw-r--r--   0 tom       (1001) nslab     (1000)     3470 2018-10-17 12:52:06.000000 npf-1.0.8/modules/fastclick-replay-txonly-mt.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     9603 2020-02-01 08:49:32.000000 npf-1.0.8/modules/fastclick-udpgen-latency-single-multiclient.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     4301 2018-05-08 09:53:43.000000 npf-1.0.8/modules/fastclick-udpgen-latency-quad.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      383 2019-03-08 11:30:22.000000 npf-1.0.8/modules/droptcpsock.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      735 2018-04-17 09:59:39.000000 npf-1.0.8/modules/fastclick-rcv.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     5474 2020-06-05 09:01:58.000000 npf-1.0.8/modules/fastclick-replay-single-pipeline.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      942 2020-09-30 17:10:13.000000 npf-1.0.8/modules/cpuload.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1023 2020-02-01 08:49:32.000000 npf-1.0.8/modules/perf-functions.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1671 2020-09-05 08:04:15.000000 npf-1.0.8/modules/wrk.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-03 13:58:24.000000 npf-1.0.8/modules/__init__.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     5886 2020-12-12 15:05:23.000000 npf-1.0.8/modules/fastclick-udpgen-latency-single.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     4499 2019-04-03 17:13:34.000000 npf-1.0.8/modules/fastclick-udpgen-dual.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    10969 2020-12-10 17:06:30.000000 npf-1.0.8/modules/fastclick-replay-single-mt.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1671 2020-11-03 17:36:17.000000 npf-1.0.8/modules/dev_rate.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     3592 2018-04-17 09:59:39.000000 npf-1.0.8/modules/fastclick-udpgen-latency-dual.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1311 2020-09-15 13:00:03.000000 npf-1.0.8/modules/load.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    12199 2020-10-02 12:00:36.000000 npf-1.0.8/modules/fastclick-play-single-mt.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      368 2019-02-13 16:44:54.000000 npf-1.0.8/modules/dev_channels.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     5446 2020-04-09 20:59:14.000000 npf-1.0.8/modules/wrk-nsdelay.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1130 2020-09-15 15:58:38.000000 npf-1.0.8/modules/cpufreq-script-half.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     9026 2018-05-08 09:53:43.000000 npf-1.0.8/modules/fastclick-replay-quad.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1313 2020-09-15 13:13:46.000000 npf-1.0.8/modules/load2.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     8771 2019-06-26 14:53:06.000000 npf-1.0.8/modules/fastclick-replay-single-mt-rated.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     8004 2018-04-17 09:59:39.000000 npf-1.0.8/modules/fastclick-replay-dual.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    29621 2018-08-14 09:12:01.000000 npf-1.0.8/modules/snort.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     5064 2020-06-05 09:01:59.000000 npf-1.0.8/modules/fastclick-replay-single.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    11227 2019-06-22 20:34:35.000000 npf-1.0.8/modules/fastclick-play-single-mt-quad.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      720 2020-09-15 22:09:24.000000 npf-1.0.8/modules/waitcon.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      929 2018-10-25 15:04:22.000000 npf-1.0.8/modules/pktgen.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      155 2018-08-15 10:25:08.000000 npf-1.0.8/modules/dev_pause.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    10614 2020-10-02 12:00:36.000000 npf-1.0.8/modules/fastclick-replay-single-multitrace.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)       37 2018-09-17 13:43:32.000000 npf-1.0.8/modules/trex.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    26521 2019-05-05 10:22:37.000000 npf-1.0.8/modules/dpdk-bind.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1818 2020-04-08 08:08:00.000000 npf-1.0.8/modules/wrk-multins.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1252 2018-04-17 09:59:39.000000 npf-1.0.8/modules/fastclick-udpgen-snd.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    11066 2018-05-08 09:53:43.000000 npf-1.0.8/modules/fastclick-replay-vmdq-quad.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     2621 2018-04-17 09:59:39.000000 npf-1.0.8/modules/fastclick-udpgen-quad.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    11787 2020-09-17 19:04:28.000000 npf-1.0.8/modules/reframer.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1876 2020-10-02 12:00:35.000000 npf-1.0.8/modules/wrk2.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     2286 2020-10-02 12:00:35.000000 npf-1.0.8/modules/cpufreq-script.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      577 2018-04-17 09:59:39.000000 npf-1.0.8/modules/cpufreq.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)      461 2017-09-14 09:21:00.000000 npf-1.0.8/modules/netmap-bind.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)    13752 2020-10-23 14:51:28.000000 npf-1.0.8/modules/fastclick-replay-single-mt-timing.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     1204 2020-01-18 10:55:31.000000 npf-1.0.8/modules/perf-class.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     3965 2020-09-14 15:21:37.000000 npf-1.0.8/modules/nginx.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     2447 2017-08-08 12:02:50.000000 npf-1.0.8/modules/fastclick-udpgen-single.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     9649 2020-09-10 10:18:58.000000 npf-1.0.8/modules/fastclick-replay-single-multitrace-tmp.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)     2896 2020-09-01 09:19:32.000000 npf-1.0.8/modules/dev_irq_affinity.npf
--rw-r--r--   0 tom       (1001) nslab     (1000)       38 2020-12-14 10:50:43.000000 npf-1.0.8/setup.cfg
--rwxr-xr-x   0 tom       (1001) nslab     (1000)    11804 2020-12-11 10:03:18.000000 npf-1.0.8/npf_run.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    17067 2020-12-01 15:00:40.000000 npf-1.0.8/README.md
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/repo/
--rw-r--r--   0 tom       (1001) nslab     (1000)      161 2017-09-14 09:21:00.000000 npf-1.0.8/repo/haproxy.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      302 2020-12-09 14:26:38.000000 npf-1.0.8/repo/fastclick.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       73 2017-05-19 20:18:03.000000 npf-1.0.8/repo/openbox.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      181 2019-03-07 17:41:50.000000 npf-1.0.8/repo/middleclick.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       72 2018-02-07 16:20:26.000000 npf-1.0.8/repo/metron-debug.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      121 2018-10-26 09:45:56.000000 npf-1.0.8/repo/fastclick-queuecount.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      134 2017-08-08 12:02:50.000000 npf-1.0.8/repo/fastclick-nobatch-nozc.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       86 2020-05-26 08:33:33.000000 npf-1.0.8/repo/fastclick-novb.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       84 2017-05-15 13:04:55.000000 npf-1.0.8/repo/click-2017.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-03 12:17:02.000000 npf-1.0.8/repo/__init__.py
--rw-r--r--   0 tom       (1001) nslab     (1000)      119 2019-10-04 15:13:07.000000 npf-1.0.8/repo/fastclick-dumpaccel.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       33 2018-08-29 12:22:32.000000 npf-1.0.8/repo/fastclick-timerp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       62 2017-08-08 12:02:50.000000 npf-1.0.8/repo/wrk2.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      121 2020-09-03 11:23:04.000000 npf-1.0.8/repo/middleclick-static.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       55 2017-05-26 19:28:49.000000 npf-1.0.8/repo/metron-parallel.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      110 2018-10-26 14:50:25.000000 npf-1.0.8/repo/fastclick-dma.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      101 2017-05-15 13:04:55.000000 npf-1.0.8/repo/fastclick-nobatch.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      166 2019-02-26 08:22:41.000000 npf-1.0.8/repo/middleclick-debug.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      115 2019-09-23 15:02:22.000000 npf-1.0.8/repo/iperf-rsspp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      121 2019-01-08 17:46:52.000000 npf-1.0.8/repo/wrk-tbarbette.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      105 2017-09-14 09:21:00.000000 npf-1.0.8/repo/dpdk-test.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       73 2020-06-26 09:22:12.000000 npf-1.0.8/repo/fastclick-clang.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       48 2018-06-12 20:31:17.000000 npf-1.0.8/repo/metron-fix.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      108 2019-10-02 16:28:36.000000 npf-1.0.8/repo/rsspp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       96 2019-02-17 10:04:26.000000 npf-1.0.8/repo/middleclick-reset.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       80 2019-02-26 05:18:14.000000 npf-1.0.8/repo/middleclick-atomic.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      171 2017-09-14 09:18:58.000000 npf-1.0.8/repo/fastclick-nobatch-nozc-fp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       97 2018-10-24 12:05:31.000000 npf-1.0.8/repo/pktgen-dpdk.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       48 2018-12-06 20:02:15.000000 npf-1.0.8/repo/metron-dev.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      245 2018-09-17 14:07:04.000000 npf-1.0.8/repo/trex.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      142 2017-09-14 09:18:58.000000 npf-1.0.8/repo/fastclick-debug.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      143 2019-05-08 10:19:43.000000 npf-1.0.8/repo/perf-class.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       32 2017-05-15 13:04:55.000000 npf-1.0.8/repo/iptables.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      274 2019-09-23 03:14:26.000000 npf-1.0.8/repo/iperf.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      249 2019-10-02 16:30:10.000000 npf-1.0.8/repo/metron.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      257 2017-08-08 12:02:50.000000 npf-1.0.8/repo/netperf.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      114 2017-08-08 12:02:50.000000 npf-1.0.8/repo/wrk.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      174 2018-09-27 10:56:34.000000 npf-1.0.8/repo/dpdk-mlx.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       52 2017-05-26 19:28:49.000000 npf-1.0.8/repo/snf.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       96 2019-02-16 10:18:24.000000 npf-1.0.8/repo/middleclick-epoch.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      410 2019-01-09 10:38:34.000000 npf-1.0.8/repo/daq.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      124 2017-05-26 19:28:49.000000 npf-1.0.8/repo/fastclick-next.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      122 2017-09-14 09:21:00.000000 npf-1.0.8/repo/netmap.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      122 2019-01-08 17:46:52.000000 npf-1.0.8/repo/wrk2-tbarbette.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      341 2017-09-14 09:18:58.000000 npf-1.0.8/repo/click.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      533 2018-10-15 07:41:19.000000 npf-1.0.8/repo/dpdk.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       80 2017-05-25 20:17:43.000000 npf-1.0.8/repo/click-dpdk.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      114 2018-12-29 22:49:45.000000 npf-1.0.8/repo/fastclick-imp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      176 2017-09-14 09:18:58.000000 npf-1.0.8/repo/fastclick-nobatch-nozc-nofp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       55 2017-05-26 19:28:49.000000 npf-1.0.8/repo/metron-pipeline.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       18 2017-05-15 13:04:55.000000 npf-1.0.8/repo/local.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      152 2019-03-01 07:18:54.000000 npf-1.0.8/repo/middleclick-dev.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)       99 2019-02-16 09:56:03.000000 npf-1.0.8/repo/middleclick-nostruct.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      101 2018-12-29 21:06:05.000000 npf-1.0.8/repo/fastclick-nofp.repo
--rw-r--r--   0 tom       (1001) nslab     (1000)      396 2018-06-13 09:14:54.000000 npf-1.0.8/repo/snort.repo
--rwxr-xr-x   0 tom       (1001) nslab     (1000)     8073 2020-12-04 11:50:55.000000 npf-1.0.8/npf_watch.py
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/npf/
--rw-r--r--   0 tom       (1001) nslab     (1000)     4453 2019-05-14 07:50:47.000000 npf-1.0.8/npf/statistics.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     1233 2019-05-05 08:23:21.000000 npf-1.0.8/npf/nic.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     8812 2020-12-11 10:03:18.000000 npf-1.0.8/npf/regression.py
--rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-03 12:17:11.000000 npf-1.0.8/npf/__init__.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     1349 2020-01-26 12:13:20.000000 npf-1.0.8/npf/eventbus.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    13415 2020-12-08 14:11:55.000000 npf-1.0.8/npf/variable.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    80801 2020-12-14 10:50:28.000000 npf-1.0.8/npf/grapher.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     4595 2020-06-05 09:02:00.000000 npf-1.0.8/npf/node.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    24564 2020-11-05 15:55:02.000000 npf-1.0.8/npf/section.py
--rwxr-xr-x   0 tom       (1001) nslab     (1000)    13436 2020-12-11 14:14:13.000000 npf-1.0.8/npf/repository.py
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/npf/executor/
--rw-r--r--   0 tom       (1001) nslab     (1000)        0 2017-05-15 13:04:55.000000 npf-1.0.8/npf/executor/__init__.py
--rw-r--r--   0 tom       (1001) nslab     (1000)      743 2020-04-24 09:32:17.000000 npf-1.0.8/npf/executor/executor.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    10827 2020-11-25 17:29:18.000000 npf-1.0.8/npf/executor/sshexecutor.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     3532 2020-10-02 12:00:35.000000 npf-1.0.8/npf/executor/localexecutor.py
--rwxr-xr-x   0 tom       (1001) nslab     (1000)    12008 2020-12-08 18:03:45.000000 npf-1.0.8/npf/build.py
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-14 10:50:43.000000 npf-1.0.8/npf/types/
--rwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2017-05-15 13:04:55.000000 npf-1.0.8/npf/types/__init__.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    12766 2020-11-05 15:58:47.000000 npf-1.0.8/npf/types/dataset.py
--rwxr-xr-x   0 tom       (1001) nslab     (1000)    61531 2020-12-11 09:39:41.000000 npf-1.0.8/npf/testie.py
--rw-r--r--   0 tom       (1001) nslab     (1000)      286 2018-04-17 09:59:40.000000 npf-1.0.8/npf/module.py
--rwxr-xr-x   0 tom       (1001) nslab     (1000)    17287 2020-12-03 12:09:22.000000 npf-1.0.8/npf/npf.py
--rw-r--r--   0 tom       (1001) nslab     (1000)     1315 2020-12-14 10:50:41.000000 npf-1.0.8/setup.py
--rw-r--r--   0 tom       (1001) nslab     (1000)    19853 2020-12-14 10:50:43.000000 npf-1.0.8/PKG-INFO
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)     7584 2020-12-04 11:50:41.000000 npf-1.0.9/npf_compare.py
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/npf.egg-info/
+-rw-r--r--   0 tom       (1001) nslab     (1000)     3291 2020-12-22 15:53:20.000000 npf-1.0.9/npf.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1001) nslab     (1000)      100 2020-12-22 15:53:20.000000 npf-1.0.9/npf.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1001) nslab     (1000)       47 2020-12-22 15:53:20.000000 npf-1.0.9/npf.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1001) nslab     (1000)      177 2020-12-22 15:53:20.000000 npf-1.0.9/npf.egg-info/requires.txt
+-rw-r--r--   0 tom       (1001) nslab     (1000)        1 2020-12-22 15:53:20.000000 npf-1.0.9/npf.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1001) nslab     (1000)    19853 2020-12-22 15:53:20.000000 npf-1.0.9/npf.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1001) nslab     (1000)       42 2020-12-03 13:57:41.000000 npf-1.0.9/MANIFEST.in
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/modules/
+-rw-r--r--   0 tom       (1001) nslab     (1000)     3470 2018-10-17 12:52:06.000000 npf-1.0.9/modules/fastclick-replay-txonly-mt.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     9603 2020-02-01 08:49:32.000000 npf-1.0.9/modules/fastclick-udpgen-latency-single-multiclient.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     4301 2018-05-08 09:53:43.000000 npf-1.0.9/modules/fastclick-udpgen-latency-quad.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      383 2019-03-08 11:30:22.000000 npf-1.0.9/modules/droptcpsock.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      735 2018-04-17 09:59:39.000000 npf-1.0.9/modules/fastclick-rcv.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     5474 2020-06-05 09:01:58.000000 npf-1.0.9/modules/fastclick-replay-single-pipeline.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      942 2020-09-30 17:10:13.000000 npf-1.0.9/modules/cpuload.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1023 2020-02-01 08:49:32.000000 npf-1.0.9/modules/perf-functions.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1671 2020-09-05 08:04:15.000000 npf-1.0.9/modules/wrk.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-03 13:58:24.000000 npf-1.0.9/modules/__init__.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     5959 2020-12-15 16:58:34.000000 npf-1.0.9/modules/fastclick-udpgen-latency-single.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     4499 2019-04-03 17:13:34.000000 npf-1.0.9/modules/fastclick-udpgen-dual.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    10969 2020-12-10 17:06:30.000000 npf-1.0.9/modules/fastclick-replay-single-mt.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1671 2020-11-03 17:36:17.000000 npf-1.0.9/modules/dev_rate.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     3592 2018-04-17 09:59:39.000000 npf-1.0.9/modules/fastclick-udpgen-latency-dual.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1311 2020-09-15 13:00:03.000000 npf-1.0.9/modules/load.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    13269 2020-12-22 10:32:07.000000 npf-1.0.9/modules/fastclick-play-single-mt.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      368 2019-02-13 16:44:54.000000 npf-1.0.9/modules/dev_channels.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     5446 2020-04-09 20:59:14.000000 npf-1.0.9/modules/wrk-nsdelay.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1130 2020-09-15 15:58:38.000000 npf-1.0.9/modules/cpufreq-script-half.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     9026 2018-05-08 09:53:43.000000 npf-1.0.9/modules/fastclick-replay-quad.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1313 2020-09-15 13:13:46.000000 npf-1.0.9/modules/load2.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     8771 2019-06-26 14:53:06.000000 npf-1.0.9/modules/fastclick-replay-single-mt-rated.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     8004 2018-04-17 09:59:39.000000 npf-1.0.9/modules/fastclick-replay-dual.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    29621 2018-08-14 09:12:01.000000 npf-1.0.9/modules/snort.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     5064 2020-12-21 17:22:14.000000 npf-1.0.9/modules/fastclick-replay-single.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      720 2020-09-15 22:09:24.000000 npf-1.0.9/modules/waitcon.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      929 2018-10-25 15:04:22.000000 npf-1.0.9/modules/pktgen.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      155 2018-08-15 10:25:08.000000 npf-1.0.9/modules/dev_pause.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    10614 2020-10-02 12:00:36.000000 npf-1.0.9/modules/fastclick-replay-single-multitrace.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)       37 2018-09-17 13:43:32.000000 npf-1.0.9/modules/trex.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    26521 2019-05-05 10:22:37.000000 npf-1.0.9/modules/dpdk-bind.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1818 2020-04-08 08:08:00.000000 npf-1.0.9/modules/wrk-multins.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1252 2018-04-17 09:59:39.000000 npf-1.0.9/modules/fastclick-udpgen-snd.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    11066 2018-05-08 09:53:43.000000 npf-1.0.9/modules/fastclick-replay-vmdq-quad.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     2621 2018-04-17 09:59:39.000000 npf-1.0.9/modules/fastclick-udpgen-quad.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    11787 2020-09-17 19:04:28.000000 npf-1.0.9/modules/reframer.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1876 2020-10-02 12:00:35.000000 npf-1.0.9/modules/wrk2.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     2286 2020-10-02 12:00:35.000000 npf-1.0.9/modules/cpufreq-script.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      577 2018-04-17 09:59:39.000000 npf-1.0.9/modules/cpufreq.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)      461 2017-09-14 09:21:00.000000 npf-1.0.9/modules/netmap-bind.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)    13752 2020-10-23 14:51:28.000000 npf-1.0.9/modules/fastclick-replay-single-mt-timing.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1204 2020-01-18 10:55:31.000000 npf-1.0.9/modules/perf-class.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     3965 2020-09-14 15:21:37.000000 npf-1.0.9/modules/nginx.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     2447 2017-08-08 12:02:50.000000 npf-1.0.9/modules/fastclick-udpgen-single.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     9649 2020-09-10 10:18:58.000000 npf-1.0.9/modules/fastclick-replay-single-multitrace-tmp.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)     2896 2020-09-01 09:19:32.000000 npf-1.0.9/modules/dev_irq_affinity.npf
+-rw-r--r--   0 tom       (1001) nslab     (1000)       38 2020-12-22 15:53:21.000000 npf-1.0.9/setup.cfg
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)    11804 2020-12-11 10:03:18.000000 npf-1.0.9/npf_run.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    17067 2020-12-01 15:00:40.000000 npf-1.0.9/README.md
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/repo/
+-rw-r--r--   0 tom       (1001) nslab     (1000)       70 2020-12-21 10:52:06.000000 npf-1.0.9/repo/fastclick-dpool.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      161 2017-09-14 09:21:00.000000 npf-1.0.9/repo/haproxy.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      302 2020-12-09 14:26:38.000000 npf-1.0.9/repo/fastclick.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       73 2017-05-19 20:18:03.000000 npf-1.0.9/repo/openbox.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      181 2019-03-07 17:41:50.000000 npf-1.0.9/repo/middleclick.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       72 2018-02-07 16:20:26.000000 npf-1.0.9/repo/metron-debug.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      121 2018-10-26 09:45:56.000000 npf-1.0.9/repo/fastclick-queuecount.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      134 2017-08-08 12:02:50.000000 npf-1.0.9/repo/fastclick-nobatch-nozc.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       86 2020-05-26 08:33:33.000000 npf-1.0.9/repo/fastclick-novb.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       84 2017-05-15 13:04:55.000000 npf-1.0.9/repo/click-2017.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-03 12:17:02.000000 npf-1.0.9/repo/__init__.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)      119 2019-10-04 15:13:07.000000 npf-1.0.9/repo/fastclick-dumpaccel.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       33 2018-08-29 12:22:32.000000 npf-1.0.9/repo/fastclick-timerp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       62 2017-08-08 12:02:50.000000 npf-1.0.9/repo/wrk2.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      121 2020-09-03 11:23:04.000000 npf-1.0.9/repo/middleclick-static.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       55 2017-05-26 19:28:49.000000 npf-1.0.9/repo/metron-parallel.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      110 2018-10-26 14:50:25.000000 npf-1.0.9/repo/fastclick-dma.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      101 2017-05-15 13:04:55.000000 npf-1.0.9/repo/fastclick-nobatch.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      166 2019-02-26 08:22:41.000000 npf-1.0.9/repo/middleclick-debug.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      115 2019-09-23 15:02:22.000000 npf-1.0.9/repo/iperf-rsspp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      121 2019-01-08 17:46:52.000000 npf-1.0.9/repo/wrk-tbarbette.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      105 2017-09-14 09:21:00.000000 npf-1.0.9/repo/dpdk-test.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       73 2020-06-26 09:22:12.000000 npf-1.0.9/repo/fastclick-clang.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       48 2018-06-12 20:31:17.000000 npf-1.0.9/repo/metron-fix.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       74 2020-12-21 11:45:57.000000 npf-1.0.9/repo/fastclick-dpacket.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      108 2019-10-02 16:28:36.000000 npf-1.0.9/repo/rsspp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       96 2019-02-17 10:04:26.000000 npf-1.0.9/repo/middleclick-reset.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       80 2019-02-26 05:18:14.000000 npf-1.0.9/repo/middleclick-atomic.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      171 2017-09-14 09:18:58.000000 npf-1.0.9/repo/fastclick-nobatch-nozc-fp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       97 2018-10-24 12:05:31.000000 npf-1.0.9/repo/pktgen-dpdk.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       48 2018-12-06 20:02:15.000000 npf-1.0.9/repo/metron-dev.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      245 2018-09-17 14:07:04.000000 npf-1.0.9/repo/trex.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      142 2017-09-14 09:18:58.000000 npf-1.0.9/repo/fastclick-debug.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      143 2019-05-08 10:19:43.000000 npf-1.0.9/repo/perf-class.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       32 2017-05-15 13:04:55.000000 npf-1.0.9/repo/iptables.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      274 2019-09-23 03:14:26.000000 npf-1.0.9/repo/iperf.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      249 2019-10-02 16:30:10.000000 npf-1.0.9/repo/metron.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      257 2017-08-08 12:02:50.000000 npf-1.0.9/repo/netperf.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      114 2017-08-08 12:02:50.000000 npf-1.0.9/repo/wrk.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      174 2018-09-27 10:56:34.000000 npf-1.0.9/repo/dpdk-mlx.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       52 2017-05-26 19:28:49.000000 npf-1.0.9/repo/snf.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       96 2019-02-16 10:18:24.000000 npf-1.0.9/repo/middleclick-epoch.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      410 2019-01-09 10:38:34.000000 npf-1.0.9/repo/daq.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      124 2017-05-26 19:28:49.000000 npf-1.0.9/repo/fastclick-next.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      122 2017-09-14 09:21:00.000000 npf-1.0.9/repo/netmap.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      122 2019-01-08 17:46:52.000000 npf-1.0.9/repo/wrk2-tbarbette.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      341 2017-09-14 09:18:58.000000 npf-1.0.9/repo/click.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      533 2018-10-15 07:41:19.000000 npf-1.0.9/repo/dpdk.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       80 2017-05-25 20:17:43.000000 npf-1.0.9/repo/click-dpdk.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      114 2018-12-29 22:49:45.000000 npf-1.0.9/repo/fastclick-imp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      176 2017-09-14 09:18:58.000000 npf-1.0.9/repo/fastclick-nobatch-nozc-nofp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       55 2017-05-26 19:28:49.000000 npf-1.0.9/repo/metron-pipeline.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       18 2017-05-15 13:04:55.000000 npf-1.0.9/repo/local.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      152 2019-03-01 07:18:54.000000 npf-1.0.9/repo/middleclick-dev.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)       99 2019-02-16 09:56:03.000000 npf-1.0.9/repo/middleclick-nostruct.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      101 2018-12-29 21:06:05.000000 npf-1.0.9/repo/fastclick-nofp.repo
+-rw-r--r--   0 tom       (1001) nslab     (1000)      396 2018-06-13 09:14:54.000000 npf-1.0.9/repo/snort.repo
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)     8073 2020-12-04 11:50:55.000000 npf-1.0.9/npf_watch.py
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/npf/
+-rw-r--r--   0 tom       (1001) nslab     (1000)     4453 2019-05-14 07:50:47.000000 npf-1.0.9/npf/statistics.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1233 2019-05-05 08:23:21.000000 npf-1.0.9/npf/nic.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     8812 2020-12-11 10:03:18.000000 npf-1.0.9/npf/regression.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-03 12:17:11.000000 npf-1.0.9/npf/__init__.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1349 2020-01-26 12:13:20.000000 npf-1.0.9/npf/eventbus.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    13415 2020-12-08 14:11:55.000000 npf-1.0.9/npf/variable.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    80801 2020-12-14 10:50:28.000000 npf-1.0.9/npf/grapher.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     4595 2020-06-05 09:02:00.000000 npf-1.0.9/npf/node.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    24564 2020-11-05 15:55:02.000000 npf-1.0.9/npf/section.py
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)    13436 2020-12-11 14:14:13.000000 npf-1.0.9/npf/repository.py
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/npf/executor/
+-rw-r--r--   0 tom       (1001) nslab     (1000)        0 2017-05-15 13:04:55.000000 npf-1.0.9/npf/executor/__init__.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)      743 2020-04-24 09:32:17.000000 npf-1.0.9/npf/executor/executor.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    10827 2020-11-25 17:29:18.000000 npf-1.0.9/npf/executor/sshexecutor.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     3532 2020-10-02 12:00:35.000000 npf-1.0.9/npf/executor/localexecutor.py
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)    12008 2020-12-08 18:03:45.000000 npf-1.0.9/npf/build.py
+drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2020-12-22 15:53:21.000000 npf-1.0.9/npf/types/
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2017-05-15 13:04:55.000000 npf-1.0.9/npf/types/__init__.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    12766 2020-11-05 15:58:47.000000 npf-1.0.9/npf/types/dataset.py
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)    61531 2020-12-11 09:39:41.000000 npf-1.0.9/npf/testie.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)      286 2018-04-17 09:59:40.000000 npf-1.0.9/npf/module.py
+-rwxr-xr-x   0 tom       (1001) nslab     (1000)    17287 2020-12-03 12:09:22.000000 npf-1.0.9/npf/npf.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)     1315 2020-12-22 15:53:00.000000 npf-1.0.9/setup.py
+-rw-r--r--   0 tom       (1001) nslab     (1000)    19853 2020-12-22 15:53:21.000000 npf-1.0.9/PKG-INFO
```

### Comparing `npf-1.0.8/npf_compare.py` & `npf-1.0.9/npf_compare.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf.egg-info/SOURCES.txt` & `npf-1.0.9/npf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 modules/cpuload.npf
 modules/dev_channels.npf
 modules/dev_irq_affinity.npf
 modules/dev_pause.npf
 modules/dev_rate.npf
 modules/dpdk-bind.npf
 modules/droptcpsock.npf
-modules/fastclick-play-single-mt-quad.npf
 modules/fastclick-play-single-mt.npf
 modules/fastclick-rcv.npf
 modules/fastclick-replay-dual.npf
 modules/fastclick-replay-quad.npf
 modules/fastclick-replay-single-mt-rated.npf
 modules/fastclick-replay-single-mt-timing.npf
 modules/fastclick-replay-single-mt.npf
@@ -85,14 +84,16 @@
 repo/daq.repo
 repo/dpdk-mlx.repo
 repo/dpdk-test.repo
 repo/dpdk.repo
 repo/fastclick-clang.repo
 repo/fastclick-debug.repo
 repo/fastclick-dma.repo
+repo/fastclick-dpacket.repo
+repo/fastclick-dpool.repo
 repo/fastclick-dumpaccel.repo
 repo/fastclick-imp.repo
 repo/fastclick-next.repo
 repo/fastclick-nobatch-nozc-fp.repo
 repo/fastclick-nobatch-nozc-nofp.repo
 repo/fastclick-nobatch-nozc.repo
 repo/fastclick-nobatch.repo
```

### Comparing `npf-1.0.8/npf.egg-info/PKG-INFO` & `npf-1.0.9/npf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npf
-Version: 1.0.8
+Version: 1.0.9
 Summary: NPF
 Home-page: https://github.com/tbarbette/npf
 Author: Tom Barbette
 Author-email: t.barbette@gmail.com
 License: UNKNOWN
 Description: Network Performance Framework
         =============================
```

### Comparing `npf-1.0.8/modules/fastclick-replay-txonly-mt.npf` & `npf-1.0.9/modules/fastclick-replay-txonly-mt.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-latency-single-multiclient.npf` & `npf-1.0.9/modules/fastclick-udpgen-latency-single-multiclient.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-latency-quad.npf` & `npf-1.0.9/modules/fastclick-udpgen-latency-quad.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-rcv.npf` & `npf-1.0.9/modules/fastclick-rcv.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-single-pipeline.npf` & `npf-1.0.9/modules/fastclick-replay-single-pipeline.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/cpuload.npf` & `npf-1.0.9/modules/cpuload.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/perf-functions.npf` & `npf-1.0.9/modules/perf-functions.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/wrk.npf` & `npf-1.0.9/modules/wrk.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-latency-single.npf` & `npf-1.0.9/modules/fastclick-udpgen-latency-single.npf`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 require_tags=import,dpdk
 
 %variables
 GEN_BURST=32
 GEN_FLOWS=128
 GEN_LENGTH=64
 GEN_BLOCKING=true
+GEN_PROMISC=false
+promisc:GEN_PROMISC=true
 PKTGEN_REPLAY_COUNT=1
 GEN_INIT_WAIT=5
 //Change not supported as of now
 GEN_THREADS=4
 -rate:LIMIT=1000000
 rate:RATE=1000
 RCV_NIC=1
@@ -69,15 +71,15 @@
 ALL_RATE=HEAD($GEN_THREADS, $ALL_RATE)
 
 ALL_LINK=EXPAND( $(gen0/rcv$NG/avg.link_rate) )
 ALL_LINK=HEAD($GEN_THREADS, $ALL_LINK)
 
 %script deps=fastclick sudo=true delay=2
 cat SPRAYER PKTGEN_CONFIG > CGEN
-$GDB click --dpdk -c 0xff -- CGEN
+$GDB click --dpdk -l 0-15 -- CGEN
 
 %sprayer:file SPRAYER
 elementclass Sprayer {
     input
     -> Strip(14)
     -> MarkIPHeader()
     -> SetIPChecksum()
@@ -117,31 +119,31 @@
     StaticThreadSched(replay $th,puller $th);
 }
 
 elementclass Receiver { $rt |
     input
     -> tsd :: TimestampDiff($rt, N $NRECORD, SAMPLE $SAMPLE ) //MT path !!
     -> Unstrip(14)
-    -> avg :: AverageCounterMP
+    -> avg :: AverageCounterIMP
     -> Discard;
 
     unt :: Print("WARNING: Untimestamped packet", -1)
     -> Discard;
     tsd[1] -> unt;
 }
 
 elementclass MultiThreadGenerator { $port, $outPort, $srcmac, $dstmac, $outSrcmac, $srcip, $dstip |
     tdOUT::ToDPDKDevice($port, BLOCKING $GEN_BLOCKING);
 
-    gen0 :: Generator(\<01>, $srcmac, $dstmac, $srcip, $dstip, 0) -> tdOUT;
-    gen1 :: Generator(\<02>, $srcmac, $dstmac, $srcip, $dstip, 1) -> tdOUT;
-    gen2 :: Generator(\<03>, $srcmac, $dstmac, $srcip, $dstip, 2) -> tdOUT;
-    gen3 :: Generator(\<04>, $srcmac, $dstmac, $srcip, $dstip, 3) -> tdOUT;
+    gen0 :: Generator(\<01>, $srcmac, $dstmac, $srcip, $dstip, 0/0) -> tdOUT;
+    gen1 :: Generator(\<02>, $srcmac, $dstmac, $srcip, $dstip, 0/1) -> tdOUT;
+    gen2 :: Generator(\<03>, $srcmac, $dstmac, $srcip, $dstip, 0/2) -> tdOUT;
+    gen3 :: Generator(\<04>, $srcmac, $dstmac, $srcip, $dstip, 0/3) -> tdOUT;
 
-    fd :: FromDPDKDevice($outPort, MAC $outSrcmac, PROMISC false, VERBOSE 99)
+    fd :: FromDPDKDevice($outPort, MAXTHREADS 4, MAC $outSrcmac, PROMISC $GEN_PROMISC, VERBOSE 99)
     -> c0 :: Classifier(12/0806 20/0001,
                         12/0806 20/0002,
                         12/0800,
                         -)[2]
     -> Strip(14)
     -> magic :: Classifier( 36/12340001,
                             36/12340002,
```

### Comparing `npf-1.0.8/modules/fastclick-udpgen-dual.npf` & `npf-1.0.9/modules/fastclick-udpgen-dual.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-single-mt.npf` & `npf-1.0.9/modules/fastclick-replay-single-mt.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/dev_rate.npf` & `npf-1.0.9/modules/dev_rate.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-latency-dual.npf` & `npf-1.0.9/modules/fastclick-udpgen-latency-dual.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/load.npf` & `npf-1.0.9/modules/load.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-play-single-mt.npf` & `npf-1.0.9/modules/fastclick-replay-single-mt-timing.npf`

 * *Files 17% similar despite different names*

```diff
@@ -8,305 +8,366 @@
 //%import@client fastclick-replay-single trace=path/to.pcap NIC=0 CLIENT_NIC=0
 
 %config
 n_retry=0
 n_runs=1
 require_tags=import,dpdk
 timeout=60
-default_role_map+={server:dut}
+default_role_map={server:dut}
 
 %variables
 PKTGEN_BURST_OUT=32
+PKTGEN_REPLAY_COUNT=1
+PKTGEN_REPLAY_TIME=0
 NIC=0
 CLIENT_NIC=0
 RCV_NIC=0
-LIMIT=50000000
-LIMIT_TIME=65
+LIMIT=500000
+TIMING=5
+TIMING_FNT=100
 GEN_THREADS=4
 PROMISC=false
 promisc:PROMISC=true
-IGNORE?=0
+IGNORE=0
+ITERATIVE=0
+iterative:ITERATIVE=1
+ITERATION_TIME=1
+END_WAIT=0
 PAUSE=none
 GEN_DESC=0
-END_AFTER=0
-GEN_RATE?=-1
-LATENCYDUMP=/tmp/latency.csv
-ITERATION_TIME?=0
-R4=15 //Monitoring thread
-
-%late_variables
-UNQUEUE=
-//unqueue :: Unqueue()
-rate:UNQUEUE=EXPAND( -> unqueue :: BandwidthRatedUnqueue($GEN_RATE, EXTRA_LENGTH true, LINK_RATE true, BURST_DURATION 1, BURST 1) )
-NRECORD=EXPAND( $(( $LIMIT  * 2 )) )
-BROADCAST_IGNORE= -> c :: Classifier(0/$mac,-) //Ignore broadcasts
-GEN_NOREWRITE_ETHER?=0
-TIMING?=false
-GEN_BLOCKING=false
-TIMING_FNT?=
-SAMPLE?=10
-DODUMP?=0
+GEN_PRINT_START=
+nolinktest=0
+largemem:DPDKMEM=127000,2000
 dump:DODUMP=1
-latval:DOLATVAL=1
-gdb:GEN_GDB=gdb -ex run -ex "signal 2" -ex "bt" -batch -args
-
+R0=0
+R1=2
+R2=4
+R3=6
+R4=8
 
-gen_nolat:DOLAT=0
-gen_nolat:GEN_TSDIFF=NoTimestampDiff
-gen_nolat:GEN_NUMBER= -> check :: CheckIPHeader(CHECKSUM false)
-gen_nolat:GEN_RECORD=
-gen_nolat:GEN_MAGIC=-> magic :: {[0]-> RoundRobinSwitch()[0-3] => [0-3]output;Idle->[4]output;}
-GEN_TSDIFF?=TimestampDiff
--gen_preped:GEN_NUMBER?= -> check :: CheckIPHeader(CHECKSUM false)  -> nPacket :: NumberPacket(42) -> StoreData(40, $magic)
-GEN_RECORD?=EXPAND(-> rt :: RecordTimestamp(N $LIMIT, OFFSET 56))
-GEN_MAGIC?=    -> magic :: Classifier( 40/5741,  40/5722,    40/57E3,      40/5774,  -);
-DOLAT?=1
-FDDISPATCH= rr :: RoundRobinSwitch;
-
-gen_preped:GEN_NUMBER= -> MarkIPHeader
-gen_preped:FDDISPATCH?=  rr :: Classifier( 40/5741,  40/5722,    40/57E3,      40/5774);
 
-
-%-rate:require
-//test $GEN_RATE -eq -1 || ( echo "GEN_RATE can only be -1 (deactivated) when rate is not given" && exit 1)
-
-%rate:require
-test $GEN_RATE -gt 1 || ( echo "GEN_RATE must be > 0" && exit 1)
+%late_variables
+GEN_HOOK?=
+SAMPLE?=1
+STARTAFTER?=0
+GEN_BLOCKING?=true
+-nodpdkload:NBBUF=EXPAND( $(( ( ( $LIMIT * $GEN_THREADS ) + (max(4096,$PKTGEN_BURST_OUT) * 2 * 8 ) ) + 8192 )) )
+-nodpdkload:ENSURE= -> EnsureDPDKBuffer
+-nodpdkload:LATEENSURE=
+nodpdkload:NBBUF=65536
+nodpdkload:ENSURE= -> MarkMACHeader()
+nodpdkload:LATEENSURE=
+DODUMP?=0
+NRECORD=EXPAND( $(( int($LIMIT / $SAMPLE * $PKTGEN_REPLAY_COUNT  * 2) )) )
+BROADCAST_IGNORE= -> c :: Classifier(0/$mac,-) //Ignore broadcasts
 
 %promisc:late_variables
 BROADCAST_IGNORE= -> c :: Classifier(-, 0/ffffffffffff)
 
-%script deps=fastclick-dumpaccel sudo=true delay=2 name=fastclick-play
-$GEN_GDB click --dpdk -l 0-15 -- PKTGEN_CONFIG
-echo "EVENT TX_FINISHED"
-echo "Generator stopped..."
+%largemem:script deps=fastclick sudo=true
+click --dpdk -l 0-15  --socket-mem $DPDKMEM --huge-dir /mnt/hugepages  -- PKTGEN_CONFIG
+
+%-largemem:script deps=fastclick sudo=true
+click --dpdk -l 0-15  -- PKTGEN_CONFIG
+//cat PKTGEN_CONFIG
+//gdb -ex run -ex "signal 2" -ex "bt" -batch -args click --dpdk -l 0-15  -- PKTGEN_CONFIG
 
 %file PKTGEN_CONFIG
-//d :: DPDKInfo($NBBUF)
+d :: DPDKInfo(NB_SOCKET_MBUF $NBBUF, NB_SOCKET_MBUF 8192)
 
 define($bout $PKTGEN_BURST_OUT)
-define($INsrcmac ${client:$CLIENT_NIC:mac})
-define($RAW_INsrcmac ${client:$CLIENT_NIC:raw_mac})
+define($INsrcmac ${self:$CLIENT_NIC:mac})
+define($RAW_INsrcmac ${self:$CLIENT_NIC:raw_mac})
 
 define($INdstmac ${server:$NIC:mac})
 define($RAW_INdstmac ${server:$NIC:raw_mac})
 
 define($ignore $IGNORE)
+define($wait 2)
 define($replay_count $PKTGEN_REPLAY_COUNT)
 define($port ${self:$RCV_NIC:pci})
 define($quick true)
 define($txverbose 99)
 define($rxverbose 99)
 
-//JiffieClock();
+HTTPServer
 
-fdIN :: FromDump($trace, STOP true, TIMING $TIMING, TIMING_FNT "$TIMING_FNT", END_AFTER $END_AFTER, ACTIVE false, BURST 1)
-tdIN :: ToDPDKDevice($port, BLOCKING $GEN_BLOCKING, BURST $bout, VERBOSE $txverbose, IQUEUE $bout, NDESC $GEN_DESC, IPCO true )
+fdIN :: FromDump($trace, STOP false, TIMING false, START_AFTER $STARTAFTER)
+tdIN :: ToDPDKDevice($port, BLOCKING $GEN_BLOCKING, BURST $bout, VERBOSE $txverbose, IQUEUE $bout, NDESC $GEN_DESC)
 
-elementclass NoTimestampDiff { $a, $b, $c, $d |
-input -> output;
-Idle->[1]output;
-}
 
 elementclass Numberise { $magic |
-    input-> Strip(14)
-    $GEN_NUMBER
-    -> ResetIPChecksum() -> Unstrip(14) -> output
+    input-> Strip(14) -> check :: CheckIPHeader(CHECKSUM false) -> nPacket :: NumberPacket(42) -> StoreData(40, $magic) -> ResetIPChecksum(L4 true) -> Unstrip(14) -> output
 }
 
-ender :: Script(TYPE PASSIVE,
-                print "Limit of $LIMIT reached",
-                stop,
-                stop);
-
 fdIN
-    -> limit   :: Counter(COUNT_CALL $LIMIT ender.run)
-    $UNQUEUE
-    -> $FDDISPATCH
+    -> rr :: PathSpinlock;
 
 elementclass Generator { $magic |
 input
-  -> replay :: Pipeliner(BLOCKING true)
-  -> EnsureDPDKBuffer
-  -> doethRewrite :: { input[0] -> active::Switch(OUTPUT $GEN_NOREWRITE_ETHER)[0] -> rwIN :: EtherRewrite($INsrcmac,$INdstmac) -> [0]output;
-  active[1] -> [0]output}
+    $ENSURE
+  //-> rwIN :: EtherRewrite($INsrcmac,$INdstmac)
   -> Pad()
   -> Numberise($magic)
+  $GEN_HOOK
+  -> replay :: ReplayUnqueue(STOP 0,STOP_TIME $PKTGEN_REPLAY_TIME, QUICK_CLONE $quick, VERBOSE true, ACTIVE true, LIMIT $LIMIT, TIMING $TIMING, BURST $PKTGEN_BURST_OUT, TIMING_FNT "$TIMING_FNT")
+    $LATEENSURE
+  -> rt :: RecordTimestamp(N $LIMIT, OFFSET 56)
   -> avgSIN :: AverageCounter(IGNORE $ignore)
-  $GEN_RECORD
+  -> avgSIN2 :: AverageCounter(IGNORE $ignore)
   -> output;
 }
 
-rr[0] -> gen0 :: Generator(\<5741>) -> tdIN;
-rr[1] -> gen1 :: Generator(\<5722>) -> tdIN;
-rr[2] -> gen2 :: Generator(\<57E3>) -> tdIN;
-rr[3] -> gen3 :: Generator(\<5774>) -> tdIN;
-
-StaticThreadSched(fdIN 0, unqueue 0)
-StaticThreadSched(gen0/replay 4)
-StaticThreadSched(gen1/replay 6)
-StaticThreadSched(gen2/replay 4)
-StaticThreadSched(gen3/replay 6)
+rr -> gen0 :: Generator(\<5601>) -> tdIN;
+rr -> gen1 :: Generator(\<5602>) -> tdIN;
+rr -> gen2 :: Generator(\<5603>) -> tdIN;
+rr -> gen3 :: Generator(\<5604>) -> tdIN;
+
+StaticThreadSched(gen0/replay $R0)
+StaticThreadSched(gen1/replay $R1)
+StaticThreadSched(gen2/replay $R2)
+StaticThreadSched(gen3/replay $R3)
 
-receiveIN :: FromDPDKDevice($port, VERBOSE $rxverbose, MAC $INsrcmac, PROMISC $PROMISC, PAUSE $PAUSE, NDESC $GEN_DESC, MAXTHREADS 4,NUMA false)
+receiveIN :: FromDPDKDevice($port, VERBOSE $rxverbose, MAC $INsrcmac, PROMISC $PROMISC, PAUSE $PAUSE, NDESC $GEN_DESC)
 
 elementclass Receiver { $mac, $dir |
     input[0]
 $BROADCAST_IGNORE
     -> Strip(14)
     -> CheckIPHeader(CHECKSUM false)
-
-$GEN_MAGIC
+    -> magic :: Classifier( 40/5601,
+                            40/5602,
+                            40/5603,
+                            40/5604,
+                            -);
 
     c[1] //Not for this computer or broadcasts
     -> Discard;
 
     magic[0]
-    -> tsdA :: $GEN_TSDIFF(gen0/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
+    -> tsdA :: TimestampDiff(gen0/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
     -> Unstrip(14)
     -> avgA :: AverageCounterMP(IGNORE $ignore)
+    -> avgA2 :: AverageCounterMP(IGNORE $ignore)
     -> Discard;
 
     magic[1]
-    -> tsdB :: $GEN_TSDIFF(gen1/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
+    -> tsdB :: TimestampDiff(gen1/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
     -> Unstrip(14)
     -> avgB :: AverageCounterMP(IGNORE $ignore)
+    -> avgB2 :: AverageCounterMP(IGNORE $ignore)
     -> Discard;
 
     magic[2]
-    -> tsdC :: $GEN_TSDIFF(gen2/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
+    -> tsdC :: TimestampDiff(gen2/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
     -> Unstrip(14)
     -> avgC :: AverageCounterMP(IGNORE $ignore)
+    -> avgC2 :: AverageCounterMP(IGNORE $ignore)
     -> Discard;
 
     magic[3]
-    -> tsdD :: $GEN_TSDIFF(gen3/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
+    -> tsdD :: TimestampDiff(gen3/rt, OFFSET 42, N $NRECORD, SAMPLE $SAMPLE )
     -> Unstrip(14)
     -> avgD :: AverageCounterMP(IGNORE $ignore)
+    -> avgD2 :: AverageCounterMP(IGNORE $ignore)
     -> Discard;
 
     magic[4]
     -> Unstrip(14)
     -> Print("WARNING: Unknown magic / untimestamped packet", -1)
     -> Discard;
 
     tsdA[1] -> Print("WARNING: Untimestamped packet on thread 0", 64) -> Discard;
     tsdB[1] -> Print("WARNING: Untimestamped packet on thread 1", 64) -> Discard;
     tsdC[1] -> Print("WARNING: Untimestamped packet on thread 2", 64) -> Discard;
     tsdD[1] -> Print("WARNING: Untimestamped packet on thread 3", 64) -> Discard;
 }
 
-ig :: Script(TYPE ACTIVE,
-    goto end $(eq $ITERATION_TIME 0),
-    set s $(now),
-    set lastcount 0,
-    set lastbytes 0,
-    set lastsent 0,
-    set last $s,
-    set indexA 0,
-    set indexB 0,
-    set indexC 0,
-    set indexD 0,
-    label loop,
-    wait ${ITERATION_TIME}s,
-    set n $(now), 
-    set t $(sub $n $s),
-    set elapsed $(sub $n $last),
-    set last $n,
-                set sent $(add $(gen0/avgSIN.count) $(gen1/avgSIN.count) $(gen2/avgSIN.count) $(gen3/avgSIN.count)),
-                set bytessent $(add $(gen0/avgSIN.byte_count) $(gen1/avgSIN.byte_count) $(gen2/avgSIN.byte_count) $(gen3/avgSIN.byte_count)),
-                set count $(add $(RIN/avgA.count) $(RIN/avgB.count) $(RIN/avgC.count) $(RIN/avgD.count)), 
-                set bytes $(add $(RIN/avgA.byte_count) $(RIN/avgB.byte_count) $(RIN/avgC.byte_count) $(RIN/avgD.byte_count)),
-                print "IG-$t-RESULT-IGCOUNT $(sub $count $lastcount)",
-                print "IG-$t-RESULT-IGISENT $(sub $sent $lastsent)",
-                print "IG-$t-RESULT-IGDROPPED $(sub $(sub $sent $count) $(sub $lastsent $lastcount))",
-                print "IG-$t-RESULT-IGTHROUGHPUT $(div $(mul $(add $(mul $(sub $count $lastcount) 24) $(sub $bytes $lastbytes)) 8) $elapsed)",
-                print "IG-$t-RESULT-IGTX $(div $(mul $(add $(mul $(sub $sent $lastsent) 24) $(sub $bytessent $lastbytessent)) 8) $elapsed)",
-                goto next $(eq $DOLAT 0),
-                print "IG-$t-RESULT-ILATENCY $(div $(add $(RIN/tsdA.average $indexA) $(RIN/tsdB.average $indexB) $(RIN/tsdC.average $indexC) $(RIN/tsdD.average $indexD)) 4)",
-                print "IG-$t-RESULT-ILAT99 $(div $(add $(RIN/tsdA.perc99 $indexA) $(RIN/tsdB.perc99 $indexB) $(RIN/tsdC.perc99 $indexC) $(RIN/tsdD.perc99 $indexD)) 4)",
-                set indexA $(RIN/tsdA.index),
-                set indexB $(RIN/tsdB.index),
-                set indexC $(RIN/tsdC.index),
-                set indexD $(RIN/tsdD.index),
-                label next,
-                set lastcount $count,
-                set lastsent $sent,
-                set lastbytes $bytes,
-                set lastbytessent $bytessent,
-    goto loop,
-    label end
-)
-
-StaticThreadSched(ig $R4);
+receiveIN -> RINswitch :: Switch(2)[0] -> RIN :: Receiver($RAW_INsrcmac,"IN");
 
-receiveIN -> RIN :: Receiver($RAW_INsrcmac,"IN");
 
-DriverManager(  print "Waiting 2 seconds before launching generation...",
+//----------------
+//Link initializer
+//----------------
+adv0 :: FastUDPFlows(RATE 0, LIMIT -1, LENGTH 64, SRCETH $INsrcmac, DSTETH $INsrcmac, SRCIP ${self:$NIC:ip}, DSTIP ${self:$NIC:ip}, FLOWS 1, FLOWSIZE 1)
+    -> advq0 :: RatedUnqueue(1)
+    -> tdIN;
+
+//Check that it received its packet from 2 outputs and emits packets on output 0 when it's the case
+linkoklock :: PathSpinlock() [0]
+  -> linkok :: Script(TYPE PACKET,
+            write advq0.active false,
+            write adv0.active false,
+            return 0
+            )
+
+
+RINswitch[2]
+    -> Classifier(0/$RAW_INsrcmac)
+    -> Print -> [0]linkoklock
+
+
+//-----------------
+
+linkok ->
+link_initialized :: Script(TYPE PACKET,
+    print "Link initialized !",
+    write RINswitch.switch -1,
+    print "IN has $(NIN/nPacket.count) packets",
+    wait 1s,
+
+    print "Starting replay...",
+    write gen0/avgSIN.reset,
+    write gen1/avgSIN.reset,
+    write gen2/avgSIN.reset,
+    write gen3/avgSIN.reset,
+    write RIN/avgA.reset,
+    write RIN/avgB.reset,
+    write RIN/avgC.reset,
+    write RIN/avgD.reset,
+    write gen0/avgSIN2.reset,
+    write gen1/avgSIN2.reset,
+    write gen2/avgSIN2.reset,
+    write gen3/avgSIN2.reset,
+    write RIN/avgA2.reset,
+    write RIN/avgB2.reset,
+    write RIN/avgC2.reset,
+    write RIN/avgD2.reset,
+    write RINswitch.switch 0 ,
+    write gen0/replay.stop $replay_count,
+    write gen1/replay.stop $replay_count,
+    write gen2/replay.stop $replay_count,
+    write gen3/replay.stop $replay_count,
+    write gen0/replay.active true,
+    write gen1/replay.active true,
+    write gen2/replay.active true,
+    write gen3/replay.active true,
+    write run_test.run 1,
+    print "Time is $(now)",
+);
+
+run_test :: Script(TYPE PASSIVE,
+            wait ${IGNORE}s,
+            print "EVENT GEN_BEGIN",
+            print "Starting bandwidth computation !",
+            print "$GEN_PRINT_START",
+            goto end $(eq $ITERATIVE 0),
+            write display_th.run 1,
+            label end)
+
+
+display_th :: Script(TYPE PASSIVE,
+                     set indexA 0,
+                     set indexB 0,
+                     set indexC 0,
+                     set indexD 0,
+                     set stime $(now),
+                     label g,
+                     write RIN/avgA.reset,
+                     write RIN/avgB.reset,
+                     write RIN/avgC.reset,
+                     write RIN/avgD.reset,
+                     write gen0/avgSIN.reset,
+                     write gen1/avgSIN.reset,
+                     write gen2/avgSIN.reset,
+                     write gen3/avgSIN.reset,
+                     wait ${ITERATION_TIME},
+                     set diff $(sub $(now) $time),
+                     print "Diff $diff",
+                     set time $(sub $(now) $stime),
+                     set tx $(add $(gen0/avgSIN.link_rate) $(gen1/avgSIN.link_rate) $(gen2/avgSIN.link_rate) $(gen3/avgSIN.link_rate)),
+                     set rx $(add $(RIN/avgA.link_rate) $(RIN/avgB.link_rate) $(RIN/avgC.link_rate) $(RIN/avgD.link_rate)),
+                     set received $(add $(RIN/avgA.count) $(RIN/avgB.count) $(RIN/avgC.count) $(RIN/avgD.count) ),
+                     set sent $(add $(gen0/avgSIN.count) $(gen1/avgSIN.count) $(gen2/avgSIN.count) $(gen3/avgSIN.count) ),
+                     print "IGEN-$time-RESULT-ICOUNT $received",
+                     print "IGEN-$time-RESULT-IDROPPED $(sub $sent $received)",
+                     print "IGEN-$time-RESULT-IDROPPEDPS $(div $(sub $sent $received) $diff)",
+                     print "IGEN-$time-RESULT-ITHROUGHPUT $rx",
+
+                     //If no packets, do not print latency
+                     goto g $(eq $(RIN/tsdA.index) $indexA),
+                     print "",
+                     print "IGEN-$time-RESULT-ILATENCY $(div $(add $(RIN/tsdA.average $indexA) $(RIN/tsdB.average $indexB) $(RIN/tsdC.average $indexC) $(RIN/tsdD.average $indexD)) 4)",
+                     print "IGEN-$time-RESULT-ILAT99 $(div $(add $(RIN/tsdA.perc99 $indexA) $(RIN/tsdB.perc99 $indexB) $(RIN/tsdC.perc99 $indexC) $(RIN/tsdD.perc99 $indexD)) 4)",
+
+                     print "IGEN-$time-RESULT-ILAT95 $(div $(add $(RIN/tsdA.perc95 $indexA) $(RIN/tsdB.perc95 $indexB) $(RIN/tsdC.perc95 $indexC) $(RIN/tsdD.perc95 $indexD)) 4)",
+
+                     print "IGEN-$time-RESULT-ILAT05 $(div $(add $(RIN/tsdA.perc 5 $indexA) $(RIN/tsdB.perc 5 $indexB) $(RIN/tsdC.perc 5 $indexC) $(RIN/tsdD.perc 5 $indexD)) 4)",
+                     print "IGEN-$time-RESULT-ITX $tx",
+                     print "IGEN-$time-RESULT-ILOSS $(sub $rx $tx)",
+
+                     set indexA $(RIN/tsdA.index),
+                     set indexB $(RIN/tsdB.index),
+                     set indexC $(RIN/tsdC.index),
+                     set indexD $(RIN/tsdD.index),
+                     
+                     goto g)
+
+StaticThreadSched(display_th $R4)
+
+RINswitch[1]->Print(LATEIN) -> Discard;
+
+DriverManager(  pause,
+                pause,
+                pause,
+                pause,
+                goto waitagain $(eq 1 0),
                 wait 2s,
-                print "Starting gen...",
-                print "EVENT GEN_BEGIN",
-                write fdIN.active true,
-                print "Starting timer wait...",
+                write advq0.active false,
+                write adv0.active false,
+                write link_initialized.run,
+                label waitagain,
                 set starttime $(now),
-                wait $LIMIT_TIME,
-                write fdIN.active 0,
+                pause,
+                pause,
+                pause,
+                pause,
                 set stoptime $(now),
-                print "EVENT GEN_DONE",
-                wait 1s,
                 print "Rate : ",
-                print $(gen0/avgSIN.link_rate),
-                print $(gen1/avgSIN.link_rate),
-                print $(gen2/avgSIN.link_rate),
-                print $(gen3/avgSIN.link_rate),
-                print $(RIN/avgA.link_rate),
-                print $(RIN/avgB.link_rate),
-                print $(RIN/avgC.link_rate),
-                print $(RIN/avgD.link_rate),
+                print $(gen0/avgSIN2.link_rate),
+                print $(gen1/avgSIN2.link_rate),
+                print $(gen2/avgSIN2.link_rate),
+                print $(gen3/avgSIN2.link_rate),
+                print $(RIN/avgA2.link_rate),
+                print $(RIN/avgB2.link_rate),
+                print $(RIN/avgC2.link_rate),
+                print $(RIN/avgD2.link_rate),
                 print "Count :",
-                print $(gen0/avgSIN.count),
-                print $(gen1/avgSIN.count),
-                print $(gen2/avgSIN.count),
-                print $(gen3/avgSIN.count),
-                print $(RIN/avgA.count),
-                print $(RIN/avgB.count),
-                print $(RIN/avgC.count),
-                print $(RIN/avgD.count),
+                print $(gen0/avgSIN2.count),
+                print $(gen1/avgSIN2.count),
+                print $(gen2/avgSIN2.count),
+                print $(gen3/avgSIN2.count),
+                print $(RIN/avgA2.count),
+                print $(RIN/avgB2.count),
+                print $(RIN/avgC2.count),
+                print $(RIN/avgD2.count),
                 read receiveIN.hw_count,
                 read receiveIN.count,
-                read receiveIN.xstats,
                 goto adump $(eq $DODUMP 0),
-                print "Dumping latency samples to $LATENCYDUMP",
                 print >$LATENCYDUMP $(RIN/tsdA.dump_list),
                 print >>$LATENCYDUMP $(RIN/tsdB.dump_list),
                 print >>$LATENCYDUMP $(RIN/tsdC.dump_list),
                 print >>$LATENCYDUMP $(RIN/tsdD.dump_list),
                 label adump,
                 print "RESULT-TESTTIME $(sub $stoptime $starttime)",
                 print "RESULT-RCVTIME $(RIN/avgA.time)",
+                 set tx $(add $(gen0/avgSIN2.link_rate) $(gen1/avgSIN2.link_rate) $(gen2/avgSIN2.link_rate) $(gen3/avgSIN2.link_rate)),
+                 set rx $(add $(RIN/avgA2.link_rate) $(RIN/avgB2.link_rate) $(RIN/avgC2.link_rate) $(RIN/avgD2.link_rate)),
+                 print "",
+                 print "RESULT-THROUGHPUT $rx",
+                 print "RESULT-TX $tx",
                 print "RESULT-LATENCY $(div $(add $(RIN/tsdA.average) $(RIN/tsdB.average) $(RIN/tsdC.average) $(RIN/tsdD.average)) 4)",
-                print "RESULT-LAT00 $(div $(add $(RIN/tsdA.min) $(RIN/tsdB.min) $(RIN/tsdC.min) $(RIN/tsdD.min)) 4)",
+/*              print "RESULT-LAT00 $(div $(add $(RIN/tsdA.min) $(RIN/tsdB.min) $(RIN/tsdC.min) $(RIN/tsdD.min)) 4)",
                 print "RESULT-LAT01 $(div $(add $(RIN/tsdA.perc01) $(RIN/tsdB.perc01) $(RIN/tsdC.perc01) $(RIN/tsdD.perc01)) 4)",
                 print "RESULT-LAT50 $(div $(add $(RIN/tsdA.median) $(RIN/tsdB.median) $(RIN/tsdC.median) $(RIN/tsdD.median)) 4)",
-                print "RESULT-LAT95 $(div $(add $(RIN/tsdA.perc95) $(RIN/tsdB.perc95) $(RIN/tsdC.perc95) $(RIN/tsdD.perc95)) 4)",
                 print "RESULT-LAT99 $(div $(add $(RIN/tsdA.perc99) $(RIN/tsdB.perc99) $(RIN/tsdC.perc99) $(RIN/tsdD.perc99)) 4)",
-                print "RESULT-LAT100 $(div $(add $(RIN/tsdA.max) $(RIN/tsdB.max) $(RIN/tsdC.max) $(RIN/tsdD.max)) 4)",
-                goto alatval $(eq ${DOLATVAL} 0),
-                set i 0,
+                print "RESULT-LAT100 $(div $(add $(RIN/tsdA.max) $(RIN/tsdB.max) $(RIN/tsdC.max) $(RIN/tsdD.max)) 4)",*/
+               /* set i 0,
                 set step 1,
                 label perc,
                 print "CDFLATVAL-$(div $(add $(RIN/tsdA.perc $i) $(RIN/tsdB.perc $i) $(RIN/tsdC.perc $i) $(RIN/tsdD.perc $i)) 4)-RESULT-CDFLATPC $(div $i 100.0)",
                 set i $(add $i $step),
                 set step $(if $(ge $i 99) 0.1 1),
                 goto perc $(le $i 100.0),
-                label alatval,
-                print "RESULT-THROUGHPUT $(add $(RIN/avgA.link_rate) $(RIN/avgB.link_rate) $(RIN/avgC.link_rate) $(RIN/avgD.link_rate) )",
-                set sent $(add $(gen0/avgSIN.count) $(gen1/avgSIN.count) $(gen2/avgSIN.count) $(gen3/avgSIN.count)),
-                set count $(add $(RIN/avgA.count) $(RIN/avgB.count) $(RIN/avgC.count) $(RIN/avgD.count)), 
-                set bytes $(add $(RIN/avgA.byte_count) $(RIN/avgB.byte_count) $(RIN/avgC.byte_count) $(RIN/avgD.byte_count)),
-                print "RESULT-COUNT $count",
-                print "RESULT-BYTES $bytes",
-                print "RESULT-SENT $sent",
-                print "RESULT-DROPPED $(sub $sent $count)",
-                print "RESULT-TX $(add $(gen0/avgSIN.link_rate)  $(gen1/avgSIN.link_rate) $(gen2/avgSIN.link_rate) $(gen3/avgSIN.link_rate))",
-                print "RESULT-PPS $(add $(RIN/avgA.rate)  $(RIN/avgB.rate) $(RIN/avgC.rate) $(RIN/avgD.rate))",
+                wait ${END_WAIT}s,*/
+                read receiveIN.xstats,
                 stop);
```

### Comparing `npf-1.0.8/modules/wrk-nsdelay.npf` & `npf-1.0.9/modules/wrk-nsdelay.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/cpufreq-script-half.npf` & `npf-1.0.9/modules/cpufreq-script-half.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-quad.npf` & `npf-1.0.9/modules/fastclick-replay-quad.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/load2.npf` & `npf-1.0.9/modules/load2.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-single-mt-rated.npf` & `npf-1.0.9/modules/fastclick-replay-single-mt-rated.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-dual.npf` & `npf-1.0.9/modules/fastclick-replay-dual.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/snort.npf` & `npf-1.0.9/modules/snort.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-single.npf` & `npf-1.0.9/modules/fastclick-replay-single.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/waitcon.npf` & `npf-1.0.9/modules/waitcon.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/pktgen.npf` & `npf-1.0.9/modules/pktgen.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-single-multitrace.npf` & `npf-1.0.9/modules/fastclick-replay-single-multitrace.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/dpdk-bind.npf` & `npf-1.0.9/modules/dpdk-bind.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/wrk-multins.npf` & `npf-1.0.9/modules/wrk-multins.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-snd.npf` & `npf-1.0.9/modules/fastclick-udpgen-snd.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-vmdq-quad.npf` & `npf-1.0.9/modules/fastclick-replay-vmdq-quad.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-quad.npf` & `npf-1.0.9/modules/fastclick-udpgen-quad.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/reframer.npf` & `npf-1.0.9/modules/reframer.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/wrk2.npf` & `npf-1.0.9/modules/wrk2.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/cpufreq-script.npf` & `npf-1.0.9/modules/cpufreq-script.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/cpufreq.npf` & `npf-1.0.9/modules/cpufreq.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/perf-class.npf` & `npf-1.0.9/modules/perf-class.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/nginx.npf` & `npf-1.0.9/modules/nginx.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-udpgen-single.npf` & `npf-1.0.9/modules/fastclick-udpgen-single.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/fastclick-replay-single-multitrace-tmp.npf` & `npf-1.0.9/modules/fastclick-replay-single-multitrace-tmp.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/modules/dev_irq_affinity.npf` & `npf-1.0.9/modules/dev_irq_affinity.npf`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf_run.py` & `npf-1.0.9/npf_run.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/README.md` & `npf-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/repo/dpdk.repo` & `npf-1.0.9/repo/dpdk.repo`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf_watch.py` & `npf-1.0.9/npf_watch.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/statistics.py` & `npf-1.0.9/npf/statistics.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/nic.py` & `npf-1.0.9/npf/nic.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/regression.py` & `npf-1.0.9/npf/regression.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/eventbus.py` & `npf-1.0.9/npf/eventbus.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/variable.py` & `npf-1.0.9/npf/variable.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/grapher.py` & `npf-1.0.9/npf/grapher.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/node.py` & `npf-1.0.9/npf/node.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/section.py` & `npf-1.0.9/npf/section.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/repository.py` & `npf-1.0.9/npf/repository.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/executor/executor.py` & `npf-1.0.9/npf/executor/executor.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/executor/sshexecutor.py` & `npf-1.0.9/npf/executor/sshexecutor.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/executor/localexecutor.py` & `npf-1.0.9/npf/executor/localexecutor.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/build.py` & `npf-1.0.9/npf/build.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/types/dataset.py` & `npf-1.0.9/npf/types/dataset.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/testie.py` & `npf-1.0.9/npf/testie.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/npf/npf.py` & `npf-1.0.9/npf/npf.py`

 * *Files identical despite different names*

### Comparing `npf-1.0.8/setup.py` & `npf-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'webcolors',
     'colorama',
     'pygtrie'
         ]
 
 setuptools.setup(
     name="npf",
-    version="1.0.8",
+    version="1.0.9",
     author="Tom Barbette",
     author_email="t.barbette@gmail.com",
     install_requires=install_requires,
     description="NPF",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tbarbette/npf",
```

### Comparing `npf-1.0.8/PKG-INFO` & `npf-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npf
-Version: 1.0.8
+Version: 1.0.9
 Summary: NPF
 Home-page: https://github.com/tbarbette/npf
 Author: Tom Barbette
 Author-email: t.barbette@gmail.com
 License: UNKNOWN
 Description: Network Performance Framework
         =============================
```

