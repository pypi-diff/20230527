# Comparing `tmp/mfhpo_simulator-0.0.3-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15442 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      483 b- defN 23-May-19 19:48 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-May-19 19:47 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx     6157 b- defN 23-May-18 10:19 benchmark_simulator/_secure_proc.py
--rw-rw-r--  2.0 unx     1846 b- defN 23-May-17 23:06 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    24059 b- defN 23-May-19 20:56 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-May-19 20:59 mfhpo_simulator-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      290 b- defN 23-May-19 20:59 mfhpo_simulator-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 20:59 mfhpo_simulator-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-May-19 20:59 mfhpo_simulator-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      871 b- defN 23-May-19 20:59 mfhpo_simulator-0.0.3.dist-info/RECORD
-10 files, 47339 bytes uncompressed, 13942 bytes compressed:  70.5%
+Zip file size: 17516 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      483 b- defN 23-May-27 14:57 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     2715 b- defN 23-May-26 21:31 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx     9482 b- defN 23-May-27 16:40 benchmark_simulator/_secure_proc.py
+-rw-rw-r--  2.0 unx     1846 b- defN 23-May-25 06:25 benchmark_simulator/_utils.py
+-rw-rw-r--  2.0 unx    27804 b- defN 23-May-27 16:40 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      871 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/RECORD
+10 files, 54380 bytes uncompressed, 16016 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-0.0.3.dist-info/LICENSE
+Filename: mfhpo_simulator-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-0.0.3.dist-info/METADATA
+Filename: mfhpo_simulator-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-0.0.3.dist-info/WHEEL
+Filename: mfhpo_simulator-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-0.0.3.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-0.0.3.dist-info/RECORD
+Filename: mfhpo_simulator-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import ObjectiveFuncType
 from benchmark_simulator.simulator import CentralWorkerManager, ObjectiveFuncWorker
 
 
-__version__ = "0.0.3"
+__version__ = "1.0.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -1,68 +1,80 @@
+from __future__ import annotations
+
 import os
-from typing import Any, Dict, NewType, Optional, Protocol, Tuple, TypedDict
+from dataclasses import dataclass
+from enum import Enum
+from typing import Any, Final, Protocol
+
+
+DIR_NAME: Final[str] = "mfhpo-simulator-info/"
+INF: Final[float] = float(1 << 30)
 
 
-class _TimeStampDictType(TypedDict):
+@dataclass(frozen=True)
+class _TimeStampDictType:
     prev_timestamp: float
     waited_time: float
 
 
+@dataclass(frozen=True)
+class _StateType:
+    runtime: float = 0.0
+    cumtime: float = 0.0
+    fidel: int = 0
+    seed: int | None = None
+
+
+class _SharedDataLocations(Enum):
+    proc_alloc: str = "proc_alloc.json"
+    result: str = "results.json"
+    state_cache: str = "state_cache.json"
+    worker_cumtime: str = "simulated_cumtime.json"
+    timestamp: str = "timestamp.json"
+
+
+class _TimeValue(Enum):
+    terminated: float = float(1 << 40)
+    crashed: float = float(1 << 41)
+
+
 class ObjectiveFuncType(Protocol):
     def __call__(
         self,
-        eval_config: Dict[str, Any],
-        fidel: Optional[int] = None,
-        seed: Optional[int] = None,
+        eval_config: dict[str, Any],
+        fidels: dict[str, int | float] | None = None,
+        seed: int | None = None,
         **data_to_scatter: Any,
-    ) -> Dict[str, float]:
+    ) -> dict[str, float]:
         """The prototype of the objective function.
 
         Args:
-            eval_config (Dict[str, Any]):
+            eval_config (dict[str, Any]):
                 The configuration to be used in the objective function.
-            fidel (Optional[int]):
-                The fidelity to be used in the objective function. Typically training epoch in deep learning.
+            fidels (Optional[dict[str, Union[float, int]]):
+                The fidelities to be used in the objective function. Typically training epoch in deep learning.
                 If None, we assume that no fidelity is used.
             seed (Optional[int]):
                 The random seed to be used in the objective function.
             **data_to_scatter (Any):
                 Data to scatter across workers.
                 For example, when the objective function instance has a large file,
                 Dask, which is a typical module for parallel optimization, must serialize/deserialize
                 the objective function instances. It causes a significant bottleneck.
                 By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
                 Note that since the handling of parallel workers vary depending on packages,
                 users must adapt by themselves.
 
         Returns:
-            results (Dict[str, float]):
+            results (dict[str, float]):
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
         raise NotImplementedError
 
 
-DIR_NAME = "mfhpo-simulator-info/"
-WORKER_CUMTIME_FILE_NAME = "simulated_cumtime.json"
-RESULT_FILE_NAME = "results.json"
-PROC_ALLOC_NAME = "proc_alloc.json"
-STATE_CACHE_FILE_NAME = "state_cache.json"
-TIMESTAMP_FILE_NAME = "timestamp.json"
-INF = 1 << 40
-_RuntimeType = NewType("_RuntimeType", float)
-_CumtimeType = NewType("_CumtimeType", float)
-_FidelityType = NewType("_FidelityType", int)
-_SeedType = NewType("_SeedType", Optional[int])  # type: ignore
-_StateType = Tuple[_RuntimeType, _CumtimeType, _FidelityType, _SeedType]
-INIT_STATE: _StateType = [0.0, 0.0, 0, None]  # type: ignore
-
-
-def _get_file_paths(dir_name: str) -> Tuple[str, str, str, str, str]:
-    return (
-        os.path.join(dir_name, PROC_ALLOC_NAME),
-        os.path.join(dir_name, RESULT_FILE_NAME),
-        os.path.join(dir_name, STATE_CACHE_FILE_NAME),
-        os.path.join(dir_name, WORKER_CUMTIME_FILE_NAME),
-        os.path.join(dir_name, TIMESTAMP_FILE_NAME),
-    )
+def _get_file_paths(dir_name: str) -> tuple[str, str, str, str, str]:
+    ret: tuple[str, str, str, str, str] = (
+        os.path.join(dir_name, fn.value) for fn in _SharedDataLocations
+    )  # type: ignore
+    return ret
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -1,34 +1,32 @@
+from __future__ import annotations
+
 import fcntl
 import os
 import time
 import warnings
-from typing import Dict, List, Optional
 
 from _io import TextIOWrapper
 
 from benchmark_simulator._constants import (
-    PROC_ALLOC_NAME,
-    RESULT_FILE_NAME,
-    STATE_CACHE_FILE_NAME,
-    TIMESTAMP_FILE_NAME,
-    WORKER_CUMTIME_FILE_NAME,
+    _SharedDataLocations,
     _StateType,
     _TimeStampDictType,
+    _TimeValue,
 )
 from benchmark_simulator._utils import secure_edit, secure_read
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
 
 def _init_simulator(dir_name: str) -> None:
-    for fn in [WORKER_CUMTIME_FILE_NAME, RESULT_FILE_NAME, STATE_CACHE_FILE_NAME, PROC_ALLOC_NAME, TIMESTAMP_FILE_NAME]:
-        path = os.path.join(dir_name, fn)
+    for fn in _SharedDataLocations:
+        path = os.path.join(dir_name, fn.value)
         with open(path, "a+") as f:
             fcntl.flock(f.fileno(), fcntl.LOCK_EX)
             f.seek(0)
             content = f.read()
             if len(content) < 2:
                 f.seek(0)
                 f.truncate()
@@ -42,87 +40,101 @@
     cur_alloc = json.load(f)
     cur_alloc[pid] = 0
     f.seek(0)
     json.dump(cur_alloc, f, indent=4)
 
 
 @secure_edit
-def _complete_proc_allocation(f: TextIOWrapper) -> Dict[int, int]:
+def _complete_proc_allocation(f: TextIOWrapper) -> dict[int, int]:
     alloc = json.load(f)
     sorted_pids = np.sort([int(pid) for pid in alloc.keys()])
     alloc = {pid: idx for idx, pid in enumerate(sorted_pids)}
     f.seek(0)
     json.dump(alloc, f, indent=4)
     return alloc
 
 
 @secure_edit
 def _record_cumtime(f: TextIOWrapper, worker_id: str, cumtime: float) -> None:
     record = json.load(f)
-    record[worker_id] = cumtime
+    prev_cumtime = record.get(worker_id, 0.0)
+    record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TimeValue.crashed.value)
     f.seek(0)
     json.dump(record, f, indent=4)
 
 
 @secure_edit
 def _record_timestamp(f: TextIOWrapper, worker_id: str, prev_timestamp: float, waited_time: float) -> None:
     record = json.load(f)
     record[worker_id] = dict(prev_timestamp=prev_timestamp, waited_time=waited_time)
     f.seek(0)
     json.dump(record, f, indent=4)
 
 
 @secure_edit
-def _cache_state(f: TextIOWrapper, config_hash: int, new_state: _StateType, update_index: Optional[int] = None) -> None:
-    cache = {int(k): v for k, v in json.load(f).items()}
-    if config_hash not in cache:
-        cache[config_hash] = [new_state]
+def _cache_state(f: TextIOWrapper, config_hash: int, new_state: _StateType, update_index: int | None = None) -> None:
+    config_hash_str = str(config_hash)
+    cache = json.load(f)
+    _new_state = [new_state.runtime, new_state.cumtime, new_state.fidel, new_state.seed]
+    if config_hash_str not in cache:
+        cache[config_hash_str] = [_new_state]
     elif update_index is not None:
-        cache[config_hash][update_index] = new_state
+        cache[config_hash_str][update_index] = _new_state
     else:
-        cache[config_hash].append(new_state)
+        cache[config_hash_str].append(_new_state)
 
     f.seek(0)
     json.dump(cache, f, indent=4)
 
 
 @secure_edit
 def _delete_state(f: TextIOWrapper, config_hash: int, index: int) -> None:
-    cache = {int(k): v for k, v in json.load(f).items()}
-    cache[config_hash].pop(index)
-    if len(cache[config_hash]) == 0:
-        cache.pop(config_hash)
+    cache = json.load(f)
+    config_hash_str = str(config_hash)
+    cache[config_hash_str].pop(index)
+    if len(cache[config_hash_str]) == 0:
+        cache.pop(config_hash_str)
 
     f.seek(0)
     json.dump(cache, f, indent=4)
 
 
 @secure_read
-def _fetch_cache_states(f: TextIOWrapper) -> Dict[int, List[_StateType]]:
-    return {int(k): v for k, v in json.load(f).items()}
+def _fetch_cache_states(f: TextIOWrapper, config_hash: int) -> list[_StateType]:
+    states = json.load(f).get(str(config_hash), [])
+    return [_StateType(runtime=state[0], cumtime=state[1], fidel=state[2], seed=state[3]) for state in states]
 
 
 @secure_read
-def _fetch_cumtimes(f: TextIOWrapper) -> Dict[str, float]:
+def _fetch_cumtimes(f: TextIOWrapper) -> dict[str, float]:
     cumtimes = json.load(f)
     return cumtimes
 
 
 @secure_read
-def _fetch_timestamps(f: TextIOWrapper) -> Dict[str, _TimeStampDictType]:
-    timestamps = json.load(f)
+def _fetch_timestamps(f: TextIOWrapper) -> dict[str, _TimeStampDictType]:
+    timestamps = {th: _TimeStampDictType(**ts_dict) for th, ts_dict in json.load(f).items()}
     return timestamps
 
 
+def _fetch_proc_alloc(path: str) -> dict[int, int]:
+    return _complete_proc_allocation(path=path)
+
+
 @secure_edit
-def _record_result(f: TextIOWrapper, results: Dict[str, float]) -> None:
+def _record_result(f: TextIOWrapper, results: dict[str, float], fixed: bool = True) -> None:
     record = json.load(f)
-    for key, val in results.items():
-        if key not in record:
+    n_observations = len(record.get("cumtime", []))
+    keys = list(set(list(record.keys()) + list(results.keys()))) if not fixed else results.keys()
+    for key in keys:
+        val = results.get(key, None)
+        if n_observations == 0:
             record[key] = [val]
+        elif key not in record:
+            record[key] = [None] * n_observations + [val]
         else:
             record[key].append(val)
 
     f.seek(0)
     json.dump(record, f, indent=4)
 
 
@@ -138,62 +150,121 @@
 
 @secure_read
 def _is_allocation_ready(f: TextIOWrapper, n_workers: int) -> bool:
     return len(json.load(f)) == n_workers
 
 
 @secure_read
-def _get_worker_id_to_idx(f: TextIOWrapper) -> Dict[str, int]:
+def _get_worker_id_to_idx(f: TextIOWrapper) -> dict[str, int]:
     return {worker_id: idx for idx, worker_id in enumerate(json.load(f).keys())}
 
 
 def _is_min_cumtime(path: str, worker_id: str) -> bool:
     cumtimes = _fetch_cumtimes(path=path)
     proc_cumtime = cumtimes[worker_id]
     return min(cumtime for cumtime in cumtimes.values()) == proc_cumtime
 
 
+def _start_timestamp(path: str, worker_id: str, prev_timestamp: float) -> None:
+    _record_timestamp(path=path, worker_id=worker_id, prev_timestamp=time.time(), waited_time=0.0)
+
+
+def _start_worker_timer(path: str, worker_id: str) -> None:
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=0.0)
+
+
+def _finish_worker_timer(path: str, worker_id: str) -> None:
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TimeValue.terminated.value)
+
+
+def _kill_worker_timer(path: str, worker_id: str) -> None:
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TimeValue.crashed.value)
+
+
+def _kill_worker_timer_with_min_cumtime(path: str) -> None:
+    cumtimes = _fetch_cumtimes(path=path)
+    worker_id = min(cumtimes, key=cumtimes.get)
+    _kill_worker_timer(path=path, worker_id=worker_id)
+
+
 def _get_timeout_message(cause: str, path: str) -> str:
     dir_name = os.path.join(*path.split("/")[:-1])
     msg = f"Timeout in {cause}. There could be two possible reasons:\n"
     msg += f"(1) The path {dir_name} already existed before the execution of the program.\n"
     msg += "(2) n_workers specified in your optimizer and that in the simulator might be different."
     return msg
 
 
 def _wait_proc_allocation(
     path: str, n_workers: int, waiting_time: float = 1e-2, time_limit: float = 10.0
-) -> Dict[int, int]:
+) -> dict[int, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
     while not _is_allocation_ready(path, n_workers=n_workers):
         time.sleep(waiting_time)
         if time.time() - start >= time_limit:
             raise TimeoutError(_get_timeout_message(cause="the allocation of procs", path=path))
 
     return _complete_proc_allocation(path)
 
 
 def _wait_all_workers(
     path: str, n_workers: int, waiting_time: float = 1e-2, time_limit: float = 10.0
-) -> Dict[str, int]:
+) -> dict[str, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
     while not _is_simulator_ready(path, n_workers=n_workers):
         time.sleep(waiting_time)
         if time.time() - start >= time_limit:
             raise TimeoutError(_get_timeout_message(cause="creating a simulator", path=path))
 
     return _get_worker_id_to_idx(path)
 
 
-def _wait_until_next(path: str, worker_id: str, waiting_time: float = 1e-4, warning_interval: int = 10) -> None:
+def _raise_unexpected_timeout_error(max_waiting_time: float) -> None:
+    raise TimeoutError(
+        f"The simulation was terminated due to too long waiting time (> {max_waiting_time} seconds). \n"
+        "You can avoid this error by setting `max_waiting_time=np.inf`,\nbut this is not recommended because "
+        "n_workers may not be consistent throughout the simulation without setting max_waiting_time.\n"
+        "The possible reasons for the termination are the following:\n"
+        "\t1. Your sampler takes too long time to sample for the provided `max_waiting_time`,\n"
+        "\t2. n_workers is too large for the provided `max_waiting_time`,\n"
+        "\t3. Some workers crashed or new workers were added, and this caused hang, or\n"
+        "\t4. The RAM usage is too high due to the benchmark dataset which you use.\n"
+        "When you get this error, please report it to our GitHub repository with the following infos:\n"
+        "\t1. Your OS and its version,\n"
+        "\t2. Python version,\n"
+        "\t3. Your optimizer package name and its internal distributed computation module, and\n"
+        "\t4. Your benchmark details.\n"
+    )
+
+
+def _terminate_with_unexpected_timeout(path: str, worker_id: str, max_waiting_time: float) -> None:
+    _kill_worker_timer(path=path, worker_id=worker_id)
+    # The worker with minimum cumlative time may be able to evaluate several HPs during the wait,
+    # but it does not matter because the timeout happens due to too long wait.
+    time.sleep(1.0)
+    _kill_worker_timer_with_min_cumtime(path=path)
+    _raise_unexpected_timeout_error(max_waiting_time=max_waiting_time)
+
+
+def _wait_until_next(
+    path: str,
+    worker_id: str,
+    waiting_time: float = 1e-4,
+    warning_interval: int = 10,
+    max_waiting_time: float = np.inf,
+) -> None:
     start = time.time()
     waiting_time *= 1 + np.random.random()
     while not _is_min_cumtime(path, worker_id=worker_id):
         time.sleep(waiting_time)
-        if int(time.time() - start + 1) % warning_interval == 0:
+        curtime = time.time()
+        if int(curtime - start + 1) % warning_interval == 0:
             warnings.warn(
-                "Workers might be hanging. Please make sure `n_evals` is smaller than the actual n_evals.\n"
+                "Workers might be hanging. Please consider setting `max_waiting_time` (< np.inf).\n"
                 "Note that if samplers or the objective function need long time (> 10 seconds), "
                 "please ignore this warning."
             )
+
+        if curtime - start > max_waiting_time:
+            _terminate_with_unexpected_timeout(path=path, worker_id=worker_id, max_waiting_time=max_waiting_time)
```

## benchmark_simulator/simulator.py

```diff
@@ -27,27 +27,27 @@
     :
     * procN_id -- workerN_id
 Note that we need this file only if we have multiple processes in one run.
 For example, when we use multiprocessing, we might need it.
 `procX_id` is fetched by `os.getpid()` and `workerX_id` is initially generated by `generate_time_hash()`.
 
 2. mfhpo-simulator-info/*/results.json
-    * obj1_name -- List[obj1 at the n-th evaluation]
-    * obj2_name -- List[obj2 at the n-th evaluation]
+    * obj1_name -- list[obj1 at the n-th evaluation]
+    * obj2_name -- list[obj2 at the n-th evaluation]
     :
-    * objM_name -- List[objM at the n-th evaluation]
-    * cumtime -- List[cumtime up to the n-th evaluation]
-    * index -- List[the index of the worker of the n-th evaluation]
+    * objM_name -- list[objM at the n-th evaluation]
+    * cumtime -- list[cumtime up to the n-th evaluation]
+    * index -- list[the index of the worker of the n-th evaluation]
 This file is necessary for post-hoc analysis.
 
 3. mfhpo-simulator-info/*/state_cache.json
-    * config1 -- List[Tuple[runtime, cumtime, fidel, seed]]
-    * config2 -- List[Tuple[runtime, cumtime, fidel, seed]]
+    * config1 -- list[tuple[runtime, cumtime, fidel, seed]]
+    * config2 -- list[tuple[runtime, cumtime, fidel, seed]]
     :
-    * configN -- List[Tuple[runtime, cumtime, fidel, seed]]
+    * configN -- list[tuple[runtime, cumtime, fidel, seed]]
 This file tells you the states of each config.
 Runtime tells how long it took to evaluate configX up to the intermediate result.
 Since we would like to use this information only for the restart of trainings,
 we discard the information after each config reaches the full-fidelity training.
 Each list gets more than two elements if evaluations of the same configs happen.
 
 4. mfhpo-simulator-info/*/simulated_cumtime.json
@@ -62,469 +62,551 @@
     * worker1_id -- {"prev_timestamp": prev_timestamp1, "waited_time": waited_time1}
     * worker1_id -- {"prev_timestamp": prev_timestamp2, "waited_time": waited_time2}
     :
     * workerN_id -- {"prev_timestamp": prev_timestampN, "waited_time": waited_timeN}
 This file tells the last checkpoint timestamp of each worker (prev_timestamp) and
 how much time each worker waited for other workers in the last call.
 """
+from __future__ import annotations
+
 import os
 import threading
 import time
+from abc import ABCMeta, abstractmethod
+from dataclasses import dataclass
 from multiprocessing import Pool
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any
 
 from benchmark_simulator._constants import (
     DIR_NAME,
     INF,
-    INIT_STATE,
     ObjectiveFuncType,
-    PROC_ALLOC_NAME,
+    _SharedDataLocations,
     _StateType,
+    _TimeStampDictType,
+    _TimeValue,
     _get_file_paths,
 )
 from benchmark_simulator._secure_proc import (
     _allocate_proc_to_worker,
     _cache_state,
     _delete_state,
     _fetch_cache_states,
     _fetch_cumtimes,
+    _fetch_proc_alloc,
     _fetch_timestamps,
+    _finish_worker_timer,
     _init_simulator,
+    _is_allocation_ready,
     _is_simulator_terminated,
     _record_cumtime,
     _record_result,
     _record_timestamp,
+    _start_timestamp,
+    _start_worker_timer,
     _wait_all_workers,
     _wait_proc_allocation,
     _wait_until_next,
 )
 from benchmark_simulator._utils import _generate_time_hash
 
 import numpy as np
 
 
-DEFAULT_SEED = 42
-
+@dataclass(frozen=True)
+class _WrapperArgs:
+    subdir_name: str
+    n_workers: int
+    obj_func: ObjectiveFuncType
+    n_actual_evals_in_opt: int
+    n_evals: int
+    obj_keys: list[str]
+    runtime_key: str
+    fidel_keys: list[str] | None
+    seed: int | None
+    continual_max_fidel: int | None
+    max_waiting_time: float
+    store_config: bool
+
+
+class _BaseWrapperInterface(metaclass=ABCMeta):
+    """A base wrapper class for each worker or manager.
+    This wrapper class serves the shared interface of worker and manager class.
+
+    Attributes:
+        dir_name (str):
+            The directory name where all the information will be stored.
+        obj_keys (list[str]):
+            The objective (or constraint) names that will be stored in the result file.
+        runtime_key (str):
+            The runtime name that will be used for the scheduling.
+        fidel_keys (list[str]):
+            The fidelity names that will be used in the input `fidels`.
+    """
 
-class ObjectiveFuncWorker:
     def __init__(
         self,
         subdir_name: str,
         n_workers: int,
         obj_func: ObjectiveFuncType,
         n_actual_evals_in_opt: int,
         n_evals: int,
-        max_fidel: Optional[int] = None,
-        obj_keys: List[str] = ["loss"][:],
+        fidel_keys: list[str] | None = None,
+        obj_keys: list[str] = ["loss"][:],
         runtime_key: str = "runtime",
-        seed: int = DEFAULT_SEED,
-        continual_eval: bool = True,
+        seed: int | None = None,
+        continual_max_fidel: int | None = None,
+        max_waiting_time: float = np.inf,
+        store_config: bool = False,
     ):
-        """A worker class for each worker.
-        This worker class is supposed to be instantiated for each worker.
-        For example, if we use 4 workers for an optimization, then four instances should be created.
+        """The initialization of a wrapper class.
+
+        Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
 
         Args:
             subdir_name (str):
                 The subdirectory name to store all running information.
             n_workers (int):
                 The number of workers to use. In other words, how many parallel workers to use.
-            func (ObjectiveFuncType):
+            obj_func (ObjectiveFuncType):
                 A callable object that serves as the objective function.
                 Args:
-                    eval_config: Dict[str, Any]
-                    fidel: int
-                    seed: Optional[int]
+                    eval_config: dict[str, Any]
+                    fidels: dict[str, int | float] | None
+                    seed: int | None
                     **data_to_scatter: Any
                 Returns:
-                    results: Dict[str, float]
+                    results: dict[str, float]
                         It must return `objective metric` and `runtime` at least.
             n_actual_evals_in_opt (int):
                 The number of evaluations that optimizers do and it is used only for raising an error in init.
                 Note that the number of evaluations means
                 how many times we call the objective function during the optimization.
                 This number is needed to automatically finish the worker class.
                 We cannot know the timing of the termination without this information, and thus optimizers hang.
             n_evals (int):
                 How many configurations we would like to collect.
                 More specifically, how many times we call the objective function during the optimization.
                 We can guarantee that `results.json` has at least this number of evaluations.
-            max_fidel (Optional[int]):
-                The maximum fidelity defined in the objective function.
+            fidel_keys (list[str] | None):
+                The fidelity names to be used in the objective function.
                 If None, we assume that no fidelity is used.
-            obj_keys (List[str]):
+            obj_keys (list[str]):
                 The keys of the objective metrics used in `results` returned by func.
             runtime_key (str):
                 The key of the runtime metric used in `results` returned by func.
-            seed (int):
+            seed (int | None):
                 The random seed to be used to allocate random seed to each call.
-            continual_eval (bool):
-                Whether each call is a continuation from the call with the same eval_config and lower fidel.
+            continual_max_fidel (int | None):
+                The maximum fidelity to used in continual evaluations.
+                This is valid only if we use a single fidelity.
+                If not None, each call is a continuation from the call with the same eval_config and lower fidel.
                 For example, when we already trained the objective with configA and training_epoch=10,
                 we probably would like to continue the training from epoch 10 rather than from scratch
                 for call with configA and training_epoch=30.
                 continual_eval=True calculates the runtime considers this.
                 If False, each call is considered to be processed from scratch.
+            max_waiting_time (float):
+                The maximum waiting time to judge hang.
+                If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
+            store_config (bool):
+                Whether to store all config/fidel information.
+                The information is sorted chronologically.
+                When you do large-scale experiments, this may incur too much storage consumption.
         """
-        self._guarantee_no_hang(n_workers=n_workers, n_actual_evals_in_opt=n_actual_evals_in_opt, n_evals=n_evals)
-        self._worker_id = _generate_time_hash()
-        self._dir_name = os.path.join(DIR_NAME, subdir_name)
-        _, self._result_path, self._state_path, self._cumtime_path, self._timestamp_path = _get_file_paths(
-            self.dir_name
+        self._wrapper_args = _WrapperArgs(
+            subdir_name=subdir_name,
+            n_workers=n_workers,
+            obj_func=obj_func,
+            n_actual_evals_in_opt=n_actual_evals_in_opt,
+            n_evals=n_evals,
+            fidel_keys=fidel_keys,
+            obj_keys=obj_keys,
+            runtime_key=runtime_key,
+            seed=seed,
+            continual_max_fidel=continual_max_fidel,
+            max_waiting_time=max_waiting_time,
+            store_config=store_config,
         )
-        self._init_worker()
-
-        self._rng = np.random.RandomState(seed)
-        self._use_fidel = max_fidel is not None
-        self._obj_func = obj_func
-        self._max_fidel, self._n_evals = max_fidel, n_evals
+        self._dir_name = os.path.join(DIR_NAME, subdir_name)
         self._obj_keys, self._runtime_key = obj_keys[:], runtime_key
-        self._index = self._alloc_index(n_workers)
-        self._cumtime = 0.0
-        self._continual_eval = continual_eval
-        self._terminated = False
-
-    def __repr__(self) -> str:
-        return f"Worker-{self._worker_id}"
+        self._fidel_keys = [] if fidel_keys is None else fidel_keys[:]
+        self._init_wrapper()
 
     @property
     def dir_name(self) -> str:
         return self._dir_name
 
     @property
-    def max_fidel(self) -> Optional[int]:
-        return self._max_fidel
+    def obj_keys(self) -> list[str]:
+        return self._obj_keys[:]
 
     @property
     def runtime_key(self) -> str:
         return self._runtime_key
 
     @property
-    def obj_keys(self) -> List[str]:
-        return self._obj_keys[:]
+    def fidel_keys(self) -> list[str]:
+        return self._fidel_keys[:]
+
+    @abstractmethod
+    def _init_wrapper(self) -> None:
+        raise NotImplementedError
+
+
+class ObjectiveFuncWorker(_BaseWrapperInterface):
+    """A worker class for each worker.
+    This worker class is supposed to be instantiated for each worker.
+    For example, if we use 4 workers for an optimization, then four instances should be created.
+    """
+
+    def _init_wrapper(self) -> None:
+        self._guarantee_no_hang()
+        self._worker_id = _generate_time_hash()
+        _, self._result_path, self._state_path, self._cumtime_path, self._timestamp_path = _get_file_paths(
+            self.dir_name
+        )
+        self._init_worker()
 
-    def _guarantee_no_hang(self, n_workers: int, n_actual_evals_in_opt: int, n_evals: int) -> None:
+        self._rng = np.random.RandomState(self._wrapper_args.seed)
+        self._use_fidel = self._wrapper_args.fidel_keys is not None
+        self._obj_func = self._wrapper_args.obj_func
+        self._stored_obj_keys = list(set(self.obj_keys + [self.runtime_key]))
+        self._index = self._alloc_index()
+        self._cumtime = 0.0
+        self._continual_eval = self._wrapper_args.continual_max_fidel is not None
+        self._terminated = False
+        self._crashed = False
+        self._used_config: dict[str, Any] = {}
+        self._validate_fidel_args()
+
+    def __repr__(self) -> str:
+        return f"Worker-{self._worker_id}"
+
+    def _query_obj_func(
+        self,
+        eval_config: dict[str, Any],
+        fidels: dict[str, int | float] | None,
+        seed: int | None,
+        **data_to_scatter: Any,
+    ) -> dict[str, float]:
+        if self._wrapper_args.store_config:
+            self._used_config = eval_config.copy()
+            self._used_config.update(**(fidels if fidels is not None else {}), seed=seed)
+
+        return self._obj_func(eval_config=eval_config, fidels=fidels, seed=seed, **data_to_scatter)
+
+    def _guarantee_no_hang(self) -> None:
+        n_workers, n_evals = self._wrapper_args.n_workers, self._wrapper_args.n_evals
+        n_actual_evals_in_opt = self._wrapper_args.n_actual_evals_in_opt
         if n_actual_evals_in_opt < n_workers + n_evals:
             threshold = n_workers + n_evals
             # In fact, n_workers + n_evals - 1 is the real minimum threshold.
             raise ValueError(
                 "Cannot guarantee that optimziers will not hang. "
                 f"Use n_actual_evals_in_opt >= {threshold} (= n_evals + n_workers) at least. "
                 "Note that our package cannot change your optimizer setting, so "
                 "make sure that you changed your optimizer setting, but not only `n_actual_evals_in_opt`."
             )
 
+    def _validate_fidel_args(self) -> None:
+        # Guarantee the sufficiency: self._continual_eval ==> len(self._fidel_keys) == 1
+        if self._continual_eval and len(self._fidel_keys) != 1:
+            raise ValueError(
+                f"continual_max_fidel is valid only if fidel_keys has only one element, but got {self._fidel_keys}"
+            )
+
     def _init_worker(self) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
         _init_simulator(dir_name=self.dir_name)
-        _record_cumtime(path=self._cumtime_path, worker_id=self._worker_id, cumtime=0.0)
+        _start_worker_timer(path=self._cumtime_path, worker_id=self._worker_id)
 
-    def _alloc_index(self, n_workers: int) -> int:
-        worker_id_to_index = _wait_all_workers(path=self._cumtime_path, n_workers=n_workers)
+    def _alloc_index(self) -> int:
+        worker_id_to_index = _wait_all_workers(path=self._cumtime_path, n_workers=self._wrapper_args.n_workers)
         time.sleep(1e-2)  # buffer before the optimization
         return worker_id_to_index[self._worker_id]
 
-    def _get_init_state(self) -> Tuple[_StateType, Optional[int]]:
-        init_state = INIT_STATE[:]
+    def _get_init_state(self) -> tuple[_StateType, int | None]:
         # initial seed, note: 1 << 30 is a huge number that fits 32bit.
-        init_state[-1] = self._rng.randint(1 << 30)  # type: ignore
+        init_state = _StateType(seed=self._rng.randint(1 << 30))
         return init_state, None
 
-    def _get_cached_state_and_index(self, config_hash: int, fidel: Optional[int]) -> Tuple[_StateType, Optional[int]]:
-        if not self._use_fidel:  # no-fidelity opt does not use cache
-            return self._get_init_state()
-
-        # _StateType = List[_RuntimeType, _CumtimeType, _FidelityType, _SeedType]
-        cached_states = _fetch_cache_states(self._state_path).get(config_hash, [])[:]
-        intermediate_avail = [state[1] <= self._cumtime and state[2] < fidel for state in cached_states]
+    def _get_cached_state_and_index(self, config_hash: int, fidel: int) -> tuple[_StateType, int | None]:
+        cached_states = _fetch_cache_states(self._state_path, config_hash=config_hash)
+        intermediate_avail = [state.cumtime <= self._cumtime and state.fidel < fidel for state in cached_states]
         cached_state_index = intermediate_avail.index(True) if any(intermediate_avail) else None
         if cached_state_index is None:
             return self._get_init_state()
         else:
-            return cached_states[cached_state_index][:], cached_state_index
+            return cached_states[cached_state_index], cached_state_index
 
     def _update_state(
         self,
         config_hash: int,
-        fidel: Optional[int],
+        fidel: int,
         total_runtime: float,
-        seed: Optional[int],
-        cached_state_index: Optional[int],
+        seed: int | None,
+        cached_state_index: int | None,
     ) -> None:
-        if not self._use_fidel:  # no-fidelity opt does not use cache
-            return
-
         kwargs = dict(path=self._state_path, config_hash=config_hash)
-        if fidel != self.max_fidel:  # update the cache data
-            new_state = [total_runtime, self._cumtime, fidel, seed]
+        if fidel != self._wrapper_args.continual_max_fidel:  # update the cache data
+            new_state = _StateType(runtime=total_runtime, cumtime=self._cumtime, fidel=fidel, seed=seed)
             _cache_state(new_state=new_state, update_index=cached_state_index, **kwargs)
         elif cached_state_index is not None:  # if None, newly start and train till the end, so no need to delete.
             _delete_state(index=cached_state_index, **kwargs)
 
-    def _validate_output(self, results: Dict[str, float]) -> None:
+    def _validate_output(self, results: dict[str, float]) -> None:
         keys_in_output = set(results.keys())
-        keys = set(self.obj_keys + [self.runtime_key])
-        print(keys_in_output.intersection(keys), keys)
+        keys = set(self._stored_obj_keys)
         if keys_in_output.intersection(keys) != keys:
             raise KeyError(
                 f"The output of objective must be a superset of {list(keys)} specified in obj_keys and runtime_key, "
                 f"but got {results}"
             )
 
-    def _proc_output(
-        self, eval_config: Dict[str, Any], fidel: Optional[int], **data_to_scatter: Any
-    ) -> Dict[str, float]:
+    def _proc_output_from_scratch(
+        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
+    ) -> dict[str, float]:
+        _fidels: dict[str, int | float] = {} if fidels is None else fidels.copy()
+        if self._use_fidel and set(_fidels.keys()) != set(self._fidel_keys):
+            raise KeyError(f"The keys in fidels must be identical to fidel_keys, but got {fidels}")
+
+        seed = self._rng.randint(1 << 30)
+        results = self._query_obj_func(eval_config=eval_config, seed=seed, fidels=fidels, **data_to_scatter)
+        self._validate_output(results)
+        self._cumtime += results[self._runtime_key]
+        return {k: results[k] for k in self._stored_obj_keys}
+
+    def _proc_output_from_existing_state(
+        self, eval_config: dict[str, Any], fidel: int, **data_to_scatter: Any
+    ) -> dict[str, float]:
         config_hash: int = hash(str(eval_config))
         cached_state, cached_state_index = self._get_cached_state_and_index(config_hash=config_hash, fidel=fidel)
-        cached_runtime, _, _, seed = cached_state
-        results = self._obj_func(
-            eval_config=eval_config, seed=seed, **(dict(fidel=fidel) if self._use_fidel else {}), **data_to_scatter
+        _fidels: dict[str, int | float] = {self._fidel_keys[0]: fidel}
+        results = self._query_obj_func(
+            eval_config=eval_config, seed=cached_state.seed, fidels=_fidels, **data_to_scatter
         )
         self._validate_output(results)
         total_runtime = results[self._runtime_key]
-        actual_runtime = max(0.0, total_runtime - cached_runtime) if self._continual_eval else total_runtime
-        self._cumtime += actual_runtime  # TODO
+        actual_runtime = max(0.0, total_runtime - cached_state.runtime)
+        self._cumtime += actual_runtime
         self._update_state(
             total_runtime=total_runtime,
             cached_state_index=cached_state_index,
-            seed=seed,
+            seed=cached_state.seed,
             config_hash=config_hash,
             fidel=fidel,
         )
         return {**{k: results[k] for k in self._obj_keys}, self._runtime_key: actual_runtime}
 
+    def _validate_provided_fidels(self, fidels: dict[str, int | float] | None) -> int:
+        if fidels is None or len(fidels.values()) != 1:
+            raise ValueError(
+                f"fidels must have only one element when continual_max_fidel is provided, but got {fidels}"
+            )
+
+        fidel = next(iter(fidels.values()))
+        if not isinstance(fidel, int):
+            raise ValueError(f"Fidelity for continual evaluation must be integer, but got {fidel}")
+        if fidel < 0:
+            raise ValueError(f"Fidelity for continual evaluation must be non-negative, but got {fidel}")
+
+        return fidel
+
+    def _proc_output(
+        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
+    ) -> dict[str, float]:
+        if not self._continual_eval:
+            return self._proc_output_from_scratch(eval_config=eval_config, fidels=fidels, **data_to_scatter)
+
+        # Otherwise, we try the continual evaluation
+        fidel = self._validate_provided_fidels(fidels)
+        return self._proc_output_from_existing_state(eval_config=eval_config, fidel=fidel, **data_to_scatter)
+
     def _wait_other_workers(self) -> None:
         """
         Wait until the worker's cumulative runtime becomes the smallest.
         The smallest cumulative runtime implies that the order in the record will not disturbed
         even if the worker reports its results now.
         """
         wait_start = time.time()
-        _wait_until_next(path=self._cumtime_path, worker_id=self._worker_id)
+        max_waiting_time = self._wrapper_args.max_waiting_time
+        _wait_until_next(path=self._cumtime_path, worker_id=self._worker_id, max_waiting_time=max_waiting_time)
         _record_timestamp(
             path=self._timestamp_path,
             worker_id=self._worker_id,
             prev_timestamp=time.time(),
             waited_time=time.time() - wait_start,
         )
 
-    def _post_proc(self, results: Dict[str, float]) -> None:
+    def _post_proc(self, results: dict[str, float]) -> None:
         # First, record the simulated cumulative runtime after calling the objective
         _record_cumtime(path=self._cumtime_path, worker_id=self._worker_id, cumtime=self._cumtime)
         # Wait till the cumulative runtime becomes the smallest
         self._wait_other_workers()
-        row = dict(cumtime=self._cumtime, index=self._index, **{k: results[k] for k in self._obj_keys})
+
+        row = dict(
+            cumtime=self._cumtime, index=self._index, **{k: results[k] for k in self._obj_keys}, **self._used_config
+        )
         # Record the results to the main database when the cumulative runtime is the smallest
-        _record_result(self._result_path, results=row)
-        if _is_simulator_terminated(self._result_path, max_evals=self._n_evals):
+        _record_result(self._result_path, results=row, fixed=bool(not self._wrapper_args.store_config))
+        self._used_config = {}  # Make it empty
+        if _is_simulator_terminated(self._result_path, max_evals=self._wrapper_args.n_evals):
             self._finish()
 
-    def _load_timestamps(self) -> Tuple[float, float]:
+    def _load_timestamps(self) -> _TimeStampDictType:
         timestamp_dict = _fetch_timestamps(self._timestamp_path)
-        if len(timestamp_dict) == 0:  # We do not need it right after the instantiation
-            return 0.0, time.time()
+        if self._worker_id not in timestamp_dict:  # Initialize the timestamp
+            init_timestamp = _TimeStampDictType(prev_timestamp=time.time(), waited_time=0.0)
+            _start_timestamp(
+                path=self._timestamp_path, worker_id=self._worker_id, prev_timestamp=init_timestamp.prev_timestamp
+            )
+            return init_timestamp
 
         timestamp = timestamp_dict[self._worker_id]
         self._cumtime = _fetch_cumtimes(self._cumtime_path)[self._worker_id]
-        self._terminated = self._cumtime >= INF - 1e-5  # INF means finish has been called.
-        return timestamp["waited_time"], timestamp["prev_timestamp"]
+        self._terminated = self._cumtime >= _TimeValue.terminated.value - 1e-5
+        self._crashed = self._cumtime >= _TimeValue.crashed.value - 1e-5
+        return timestamp
+
+    def _validate(self, fidels: dict[str, int | float] | None) -> None:
+        if self._crashed:
+            raise InterruptedError(
+                "The simulation is interrupted due to deadlock or the dead of at least one of the workers.\n"
+                "This error could be avoided by increasing `max_waiting_time` (however, np.inf is discouraged).\n"
+            )
+        if not self._use_fidel and fidels is not None:
+            raise ValueError(
+                "Objective function got keyword `fidels`, but fidel_keys was not provided in worker instantiation."
+            )
+        if self._use_fidel and fidels is None:
+            raise ValueError(
+                "Objective function did not get keyword `fidels`, but fidel_keys was provided in worker instantiation."
+            )
 
     def __call__(
-        self, eval_config: Dict[str, Any], fidel: Optional[int] = None, **data_to_scatter: Any
-    ) -> Dict[str, float]:
+        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None = None, **data_to_scatter: Any
+    ) -> dict[str, float]:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
         If not called, optimization modules are likely to hang at the end.
 
         Args:
-            eval_config (Dict[str, Any]):
+            eval_config (dict[str, Any]):
                 The configuration to be used in the objective function.
-            fidel (Optional[int]):
-                The fidelity to be used in the objective function. Typically training epoch in deep learning.
+            fidels (dict[str, int | float] | None):
+                The fidelities to be used in the objective function. Typically training epoch in deep learning.
                 If None, no-fidelity opt.
             **data_to_scatter (Any):
                 Data to scatter across workers.
                 For example, when the objective function instance has a large file,
                 Dask, which is a typical module for parallel optimization, must serialize/deserialize
                 the objective function instances. It causes a significant bottleneck.
                 By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
                 Note that since the handling of parallel workers vary depending on packages,
                 users must adapt by themselves.
 
         Returns:
-            results (Dict[str, float]):
+            results (dict[str, float]):
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
-        waited_time, prev_timestamp = self._load_timestamps()
+        timestamp = self._load_timestamps()
+        self._validate(fidels=fidels)
         if self._terminated:
             return {**{k: INF for k in self._obj_keys}, self._runtime_key: INF}
-        if self.max_fidel is None and fidel is not None:
-            raise ValueError(
-                "Objective function got keyword `fidel`, but max_fidel was not provided in worker instantiation."
-            )
 
-        sampling_time = max(0.0, time.time() - prev_timestamp - waited_time)
-        self._cumtime += sampling_time  # TODO
+        sampling_time = max(0.0, time.time() - timestamp.prev_timestamp - timestamp.waited_time)
+        self._cumtime += sampling_time
 
-        results = self._proc_output(eval_config, fidel, **data_to_scatter)
+        results = self._proc_output(eval_config, fidels, **data_to_scatter)
         self._post_proc(results)
         return results
 
     def _finish(self) -> None:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
         If not called, optimization modules are likely to hang.
         """
-        _record_cumtime(path=self._cumtime_path, worker_id=self._worker_id, cumtime=INF)
+        _finish_worker_timer(path=self._cumtime_path, worker_id=self._worker_id)
         self._terminated = True
 
 
-class CentralWorkerManager:
-    def __init__(
-        self,
-        subdir_name: str,
-        n_workers: int,
-        obj_func: ObjectiveFuncType,
-        n_actual_evals_in_opt: int,
-        n_evals: int,
-        max_fidel: Optional[int] = None,
-        obj_keys: List[str] = ["loss"][:],
-        runtime_key: str = "runtime",
-        seeds: Optional[List[int]] = None,
-        continual_eval: bool = True,
-    ):
-        """A central worker manager class.
-        This class is supposed to be instantiated if the optimizer module uses multiprocessing.
-        For example, Dask, multiprocessing, and joblib would need this class.
-        This class recognizes each worker by process ID.
-        Therefore, process ID for each worker must be always unique and identical.
+class CentralWorkerManager(_BaseWrapperInterface):
+    """A central worker manager class.
+    This class is supposed to be instantiated if the optimizer module uses multiprocessing.
+    For example, Dask, multiprocessing, and joblib would need this class.
+    This class recognizes each worker by process ID.
+    Therefore, process ID for each worker must be always unique and identical.
+    """
 
-        Args:
-            subdir_name (str):
-                The subdirectory name to store all running information.
-            n_workers (int):
-                The number of workers to use. In other words, how many parallel workers to use.
-            obj_func (ObjectiveFuncType):
-                A callable object that serves as the objective function.
-                Args:
-                    eval_config: Dict[str, Any]
-                    fidel: int
-                    seed: Optional[int]
-                    **data_to_scatter: Any
-                Returns:
-                    results: Dict[str, float]
-                        It must return `objective metric` and `runtime` at least.
-            n_evals (int):
-                How many configurations we evaluate.
-                More specifically, how many times we call the objective function during the optimization.
-            max_fidel (Optional[int]):
-                The maximum fidelity defined in the objective function.
-                If None, we assume that no fidelity is used.
-            obj_keys (List[str]):
-                The keys of the objective metrics used in `results` returned by func.
-            runtime_key (str):
-                The key of the runtime metric used in `results` returned by func.
-            continual_eval (bool):
-                Whether each call is a continuation from the call with the same eval_config and lower fidel.
-                For example, when we already trained the objective with configA and training_epoch=10,
-                we probably would like to continue the training from epoch 10 rather than from scratch
-                for call with configA and training_epoch=30.
-                continual_eval=True calculates the runtime considers this.
-                If False, each call is considered to be processed from scratch.
-        """
-        worker_kwargs = dict(
-            obj_func=obj_func,
-            n_workers=n_workers,
-            subdir_name=subdir_name,
-            max_fidel=max_fidel,
-            n_actual_evals_in_opt=n_actual_evals_in_opt,
-            n_evals=n_evals,
-            obj_keys=obj_keys[:],
-            runtime_key=runtime_key,
-            continual_eval=continual_eval,
-        )
-        self._obj_keys, self._runtime_key = obj_keys[:], runtime_key
-        self._dir_name = os.path.join(DIR_NAME, subdir_name)
-        self._n_workers = n_workers
-        self._workers: List[ObjectiveFuncWorker]
+    def _init_wrapper(self) -> None:
+        self._workers: list[ObjectiveFuncWorker]
         self._main_pid = os.getpid()
-        self._init_workers(worker_kwargs, seeds=seeds)
+        self._init_workers()
+        self._pid_to_index: dict[int, int] = {}
 
-        self._max_fidel = max_fidel
-        self._dir_name = self._workers[0].dir_name
-        self._pid_to_index: Dict[int, int] = {}
-
-    @property
-    def dir_name(self) -> str:
-        return self._dir_name
-
-    @property
-    def max_fidel(self) -> Optional[int]:
-        return self._max_fidel
-
-    @property
-    def runtime_key(self) -> str:
-        return self._runtime_key
-
-    @property
-    def obj_keys(self) -> List[str]:
-        return self._obj_keys[:]
-
-    def _init_workers(self, worker_kwargs: Dict[str, Any], seeds: Optional[List[int]]) -> None:
-        seeds = [DEFAULT_SEED] * self._n_workers if seeds is None else seeds[:]
-        if len(seeds) != self._n_workers:
-            raise ValueError(f"The length of seeds must be n_workers={self._n_workers}, but got seeds={seeds}")
+    def _init_workers(self) -> None:
         if os.path.exists(self.dir_name):
             raise FileExistsError(f"The directory `{self.dir_name}` already exists. Remove it first.")
 
         pool = Pool()
         results = []
-        for _, seed in enumerate(seeds):
-            results.append(pool.apply_async(ObjectiveFuncWorker, kwds=dict(**worker_kwargs, seed=seed)))
+        for _ in range(self._wrapper_args.n_workers):
+            results.append(pool.apply_async(ObjectiveFuncWorker, kwds=self._wrapper_args.__dict__))
 
         pool.close()
         pool.join()
         self._workers = [result.get() for result in results]
 
     def _init_alloc(self, pid: int) -> None:
-        _path = os.path.join(self._dir_name, PROC_ALLOC_NAME)
-        _allocate_proc_to_worker(path=_path, pid=pid)
-        self._pid_to_index = _wait_proc_allocation(path=_path, n_workers=self._n_workers)
+        _path = os.path.join(self._dir_name, _SharedDataLocations.proc_alloc.value)
+        if not _is_allocation_ready(path=_path, n_workers=self._wrapper_args.n_workers):
+            _allocate_proc_to_worker(path=_path, pid=pid)
+            self._pid_to_index = _wait_proc_allocation(path=_path, n_workers=self._wrapper_args.n_workers)
+        else:
+            self._pid_to_index = _fetch_proc_alloc(path=_path)
 
     def __call__(
-        self, eval_config: Dict[str, Any], fidel: Optional[int] = None, **data_to_scatter: Any
-    ) -> Dict[str, float]:
-        """The memta-wrapper method of the objective function method in WorkerFunc instances.
+        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None = None, **data_to_scatter: Any
+    ) -> dict[str, float]:
+        """The meta-wrapper method of the objective function method in WorkerFunc instances.
 
         This method recognizes each WorkerFunc by process ID and call the corresponding worker based on the ID.
 
         Args:
-            eval_config (Dict[str, Any]):
+            eval_config (dict[str, Any]):
                 The configuration to be used in the objective function.
-            fidel (Optional[int]):
-                The fidelity to be used in the objective function. Typically training epoch in deep learning.
+            fidels (dict[str, int | float] | None):
+                The fidelities to be used in the objective function. Typically training epoch in deep learning.
                 If None, no-fidelity opt.
             **data_to_scatter (Any):
                 Data to scatter across workers.
                 For example, when the objective function instance has a large file,
                 Dask, which is a typical module for parallel optimization, must serialize/deserialize
                 the objective function instances. It causes a significant bottleneck.
                 By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
                 Note that since the handling of parallel workers vary depending on packages,
                 users must adapt by themselves.
 
         Returns:
-            results (Dict[str, float]):
+            results (dict[str, float]):
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
         pid = os.getpid()
         pid = threading.get_ident() if pid == self._main_pid else pid
-        if len(self._pid_to_index) != self._n_workers:
+        if len(self._pid_to_index) != self._wrapper_args.n_workers:
             self._init_alloc(pid)
 
+        if pid not in self._pid_to_index:
+            raise ProcessLookupError(
+                f"An unknown process/thread with ID {pid} was specified.\n"
+                "It is likely that one of the workers crashed and a new worker was added.\n"
+                f"However, worker additions are not allowed in {self.__class__.__name__}."
+            )
+
         worker_index = self._pid_to_index[pid]
-        results = self._workers[worker_index](eval_config=eval_config, fidel=fidel, **data_to_scatter)
+        results = self._workers[worker_index](eval_config=eval_config, fidels=fidels, **data_to_scatter)
         return results
```

## Comparing `mfhpo_simulator-0.0.3.dist-info/LICENSE` & `mfhpo_simulator-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

