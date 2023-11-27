# serilog-sinks-redis

Since the main repository is inactive -> [https://github.com/dburriss/serilog-sinks-redis]

I decided to detach my pull requests from it and make this repository independent.

I am a Serilog sink for Redis List, now mantained from Turrican.

| DEV |MASTER|BLEEDING|NUGET|
|-----|------|--------|-----|
|[![CI status][1]][2]|[![Release Build status][3]][4]|[![MyGet CI][5]][6]|[![NuGet CI][7]][8]|

## Usage

> Install-Package Serilog.Sinks.Redis.List

```csharp
Log.Logger = new LoggerConfiguration()
            .WriteTo.RedisList("localhost:6379", "MyConsoleApp")
            .CreateLogger();
```

[1]: https://ci.appveyor.com/api/projects/status/pmgou6qm452s50d0?svg=true
[2]: https://ci.appveyor.com/project/dburriss/serilog-sinks-redis
[3]: https://ci.appveyor.com/api/projects/status/pmgou6qm452s50d0/branch/master?svg=true
[4]: https://ci.appveyor.com/project/dburriss/serilog-sinks-redis/branch/master
[5]: https://img.shields.io/myget/dburriss-ci/vpre/Serilog.Sinks.Redis.List.svg
[6]: http://myget.org/gallery/dburriss-ci
[7]: https://img.shields.io/nuget/v/Serilog.Sinks.Redis.List.svg
[8]: https://www.nuget.org/packages/Serilog.Sinks.Redis.List/
