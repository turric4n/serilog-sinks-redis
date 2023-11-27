# serilog-sinks-redis

Since the main repository is inactive -> [https://github.com/dburriss/serilog-sinks-redis]

I decided to detach my pull requests from it and make this repository independent.

I am a Serilog sink for Redis List, now mantained from Turrican.

## Usage

> Install-Package Serilog.Sinks.Redis.List

```csharp
Log.Logger = new LoggerConfiguration()
            .WriteTo.RedisList("localhost:6379", "MyConsoleApp")
            .CreateLogger();
```
