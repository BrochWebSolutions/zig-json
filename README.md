Each command was run several times, with the best time taken. The zsh `time` utility with a `$TIMEFMT` that shows memory was used for benchmarking.

| file                     | json implementation | max memory (KB) | time (secs) |
|:------------------------:|:-------------------:|:---------------:|:-----------:|
| tests/ascii_strings.json | zig-json            | 102000          | 0.077       |
| tests/ascii_strings.json | std.json            | 125808          | 0.367       |
| tests/numbers.json       | zig-json            | 94336           | 0.108       |
| tests/numbers.json       | std.json            | 276336          | 0.218       |
| tests/random.json        | zig-json            | 212448          | 0.301       |
| tests/random.json        | std.json            | 428114          | 0.602       |
| tests/food.json          | zig-json            | 1488            | 0.003       |
| tests/food.json          | std.json            | 1600            | 0.003       |
| tests/geojson.json       | zig-json            | 2480            | 0.007       |
| tests/geojson.json       | std.json            | 3056            | 0.008       |

