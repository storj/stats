Storj Public Network Statistics
===================================

This website provides official public statistics from Storj satellites.

The statistics are provided in JSON format. See below.

The data is updated every hour. Check the _Last-Modified_ header of the HTTP response for the exact time of the last update.

Visit the GitHub repo at [https://github.com/storj/stats](https://github.com/storj/stats) to report issues or enhancement requests.

Visit [https://storjstats.info](https://storjstats.info) to see a nice Grafana dashboard of the data. Created by the Storj forum member [Arkina](https://forum.storj.io/u/Arkina).

---

[data.json](./data.json)
------------------------

Statistics about stored and transferred data:

- **bandwidth_bytes_downloaded** - number of bytes downloaded (egress) from the network for the last 30 days
- **bandwidth_bytes_uploaded** - number of bytes uploaded (ingress) to the network for the last 30 days
- **storage_free_capacity_estimate_bytes** - statistical estimate of free storage node capacity, with suspicious values removed
- **storage_free_capacity_estimate_vetted_bytes** - statistical estimate of free storage node capacity considering only vetted nodes
- **storage_inline_bytes** - number of bytes stored in inline segments on the satellite
- **storage_inline_segments** - number of segments stored inline on the satellite
- **storage_median_healthy_pieces_count** - median number of healthy pieces per segment stored on storage nodes
- **storage_min_healthy_pieces_count** - minimum number of healthy pieces per segment stored on storage nodes
- **storage_remote_bytes** - number of bytes stored on storage nodes (does not take into account the expansion factor of erasure encoding)
- **storage_remote_segments_unavailable** - number of segments that the repairer could not download at moment, usually due to network problems.
- **storage_remote_segments** - number of segments stored on storage nodes
- **storage_total_bytes_after_expansion** -  total number of bytes stored on the network after expansion by erasure coding
- **storage_total_bytes** - total number of bytes (both inline and remote) stored on the network
- **storage_total_objects** - total number of objects stored on the network
- **storage_total_pieces** - total number of pieces stored on storage nodes
- **storage_total_segments** - total number of segments stored on storage nodes

---

[nodes.json](./nodes.json)
--------------------------

Statistics about storage nodes:

- **active_nodes** - number of storage nodes that were successfully contacted within the last 4 hours, excludes disqualified and exited nodes
- **disqualified_nodes** - number of disqualified storage nodes
- **exited_nodes** - number of storage nodes that gracefully exited the satellite, excludes disqualified nodes
- **offline_nodes** - number of storage nodes that were not successfully contacted within the last 4 hours, excludes disqualified and exited nodes
- **suspended_nodes** - number of suspended storage nodes, excludes disqualified and exited nodes
- **total_nodes** - total number of unique storage nodes that ever contacted the satellite
- **vetted_nodes** - number of vetted storage nodes, excludes disqualified and exited nodes
- **full_nodes** - number of storage nodes without free disk
- **active_wallets** - number of active wallets
- **payout** - node operators payouts in USD dollars (historical)

---
[nodes_geo.json](./nodes_geo.json)
--------------------------

Statistics about storage nodes geolocation:

- **locations** - geolocation of active storage nodes. The geolocation data is updated every 24 hours.

---

[accounts.json](./accounts.json)
--------------------------------

Statistics about user accounts:

- **registered_accounts** - number of registered user accounts

---

_This website is hosted on Storj._
