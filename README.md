# psutil.cr

[![CI](https://github.com/Green-Edge/psutil.cr/actions/workflows/ci.yml/badge.svg)](https://github.com/Green-Edge/psutil.cr/actions/workflows/ci.yml)

This is a fork of
[`aablinov/psutil.cr`](https://github.com/aablinov/psutil.cr),
originally a port of gopsutil
[Gopsutil](https://github.com/shirou/gopsutil) a library for accessing
information from the system for statistical purposes. It could be used
for software that monitors the system for alerting or graphing
purposes.

This fork fixes some issues with later versions of Crystal, and is
compatible with Crystal 1.1.1.

## Status

### OS support

- [x] Linux
- [ ] OSX

### Feature support

- [x] cpu_times
- [x] virtual_memory
- [x] disk_partitions
- [x] disk_usage
- [x] disk_io_counters
- [x] host_info
- [x] load_avg
- [x] net_io_counters

## Installation

Add this to your application's `shard.yml`:

```yaml
dependencies:
  psutil:
    github: Green-Edge/psutil.cr
```

## Usage

```crystal
require "psutil"

puts Psutil.cpu_times
puts Psutil.virtual_memory
puts Psutil.disk_partitions
puts Psutil.disk_usage
puts Psutil.disk_io_counters
puts Psutil.host_info
puts Psutil.load_avg
puts Psutil.net_io_counters
```

## Development

```
crystal spec -v
```

## Contributing

1. [Fork it](https://github.com/Green-Edge/psutil.cr/fork)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new [Pull Request](https://github.com/Green-Edge/psutil.cr/pulls)

## Contributors

- [kodnaplakal](https://github.com/kodnaplakal): Andrey Blinov - creator, maintainer
- [Green Edge](https://github.com/Green-Edge): [Phillip Oldham](https://github.com/OldhamMade) - contributor
