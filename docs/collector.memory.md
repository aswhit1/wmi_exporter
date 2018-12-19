# memory collector

The memory collector exposes metrics about system memory usage

Metric name prefix  | `memory`
Classes             | `Win32_PerfRawData_PerfOS_Memory`
Enabled by default? | Yes

## Flags

None

## Metrics

Name | Description | Type | Labels
-----|-------------|------|-------
`wmi_cs_logical_processors` | Number of installed logical processors | gauge | None
`wmi_cs_physical_memory_bytes` | Total installed physical memory | gauge | None
`wmi_memory_available_bytes` | Amount of physical memory in bytes available to processes running on the computer. This value is calculated by summing space on the Zeroed, Free, and Standby memory lists. Free memory is ready for use; Zeroed memory is pages of memory filled with zeros to prevent later processes from seeing data used by a previous process. Standby memory is memory removed from a process's working set (its physical memory) on route to disk, but is still available to be recalled. This property displays the last observed value only; it is not an average. | gauge | None
`wmi_memory_cache_bytes` | Number of bytes currently being used by the file system cache. The file system cache is an area of physical memory that stores recently used pages of data for applications. The operating system continually adjusts the size of the cache, making it as large as it can while still preserving the minimum required number of available bytes for processes. This property displays the last observed value only; it is not an average. | gauge | None
`wmi_memory_cache_bytes_peak` | Maximum number of CacheBytes after the system was last restarted. This value might be larger than the current size of the cache. CacheBytes is the sum of the System Cache Resident Bytes, System Driver Resident Bytes, System Code Resident Bytes, and Pool Paged Resident Bytes counters. This property displays the last observed value only; it is not an average. | gauge | None
`wmi_memory_cache_faults_total` | Number of faults which occur when a page sought in the file system cache is not found there and must be retrieved from elsewhere in memory (soft fault) or from disk (hard fault). The file system cache is an area of physical memory that stores recently used pages of data for applications. Cache activity is a reliable indicator of most application I/O operations. This property counts the number of faults without regard for the number of pages faulted in each operation. | gauge | None
`wmi_memory_commit_limit` | Amount of virtual memory, in bytes, that can be committed without having to extend the paging file(s). (Committed memory is physical memory for which space has been reserved on the disk paging files. Each logical disk drive has one paging file.) If the paging file(s) are be expanded, the CommitLimit value increases accordingly. This property displays the last observed value only; it is not an average. | gauge | None
`wmi_memory_committed_bytes` | Amount of committed virtual memory, in bytes. Committed memory is physical memory for which space has been reserved on the disk paging file in case it must be written back to disk. This property displays the last observed value only; it is not an average. | gauge | None
`wmi_memory_demand_zero_faults_total` | The number of zeroed pages required to satisfy faults. Zeroed pages, pages emptied of previously stored data and filled with zeros, are a security feature of Windows that prevent processes from seeing data stored by earlier processes that used the memory space | gauge | None
`wmi_memory_free_and_zero_page_list_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_free_system_page_table_entries` | Number of page table entries not being used by the system. This property displays the last observed value only; it is not an average. | gauge | None
`wmi_memory_modified_page_list_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_page_faults_total` | _Not yet documented_ | gauge | None
`wmi_memory_swap_page_reads_total` | Number of disk page reads (a single read operation reading several pages is still only counted once) | gauge | None
`wmi_memory_swap_pages_read_total` | Number of pages read across all page reads (ie counting all pages read even if they are read in a single operation) | gauge | None
`wmi_memory_swap_pages_written_total` | Number of pages written across all page writes (ie counting all pages written even if they are written in a single operation) | gauge | None
`wmi_memory_swap_page_operations_total` | Total number of swap page read and writes (PagesPersec) | gauge | None
`wmi_memory_swap_page_writes_total` | Number of disk page writes (a single write operation writing several pages is still only counted once) | gauge | None
`wmi_memory_pool_nonpaged_allocs_total` | The number of calls to allocate space in the nonpaged pool. The nonpaged pool is an area of system memory area for objects that cannot be written to disk, and must remain in physical memory as long as they are allocated | gauge | None
`wmi_memory_pool_nonpaged_bytes_total` | _Not yet documented_ | gauge | None
`wmi_memory_pool_paged_allocs_total` | _Not yet documented_ | gauge | None
`wmi_memory_pool_paged_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_pool_paged_resident_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_standby_cache_core_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_standby_cache_normal_priority_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_standby_cache_reserve_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_system_cache_resident_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_system_code_resident_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_system_code_total_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_system_driver_resident_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_system_driver_total_bytes` | _Not yet documented_ | gauge | None
`wmi_memory_transition_faults_total` | _Not yet documented_ | gauge | None
`wmi_memory_transition_pages_repurposed_total` | _Not yet documented_ | gauge | None
`wmi_memory_write_copies_total` | The number of page faults caused by attempting to write that were satisfied by copying the page from elsewhere in physical memory | gauge | None

### Example metric
_This collector does not yet have explained examples, we would appreciate your help adding them!_

## Useful queries
_This collector does not yet have any useful queries added, we would appreciate your help adding them!_

## Alerting examples
_This collector does not yet have alerting examples, we would appreciate your help adding them!_
