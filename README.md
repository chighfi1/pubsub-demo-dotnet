# Pub/Sub Demo using .NET 6
## Description

This is a .NET 6 console application that demonstrates how [Ably](https://ably.com) can be used for pub/sub messaging. You can read all about this demo in this [blog post](https://ably.com/blog/use-pub-sub-to-build-a-chat-app-with-csharp-net).

## Tech stack

The project uses the following components:

- [.NET 6](https://dotnet.microsoft.com/download/dotnet/6.0), .NET 6 SDK.
- [Spectre.Console](https://spectreconsole.net/), a library to make beautiful console applications.
- [Ably](https://ably.com/?utm_campaign=GLB-2203-pubsub-demo-dotnet&utm_content=repo-pubsub-demo-dotnet&utm_source=github&utm_medium=repo&src=GLB-2203-pubsub-demo-dotnet-github), for real-time messaging at scale.

## Building & running locally

### Prerequisites

1. Install the [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0) .


### Building & running the project

1. Build the console app by running `dotnet build` in the `src\ConsoleChat` folder.
   > The executable is located in the `src\ConsoleChat\bin\Debug\net6.0` folder.

2. Run the [`dotnet publish`](https://docs.microsoft.com/en-us/dotnet/core/tools/dotnet-publish) command:

    ```shell
    dotnet publish
    ```


Start one instance of the application in the publisher mode by going to the directory where the aforomentioned executable is located:

    ```powershell
    .\ConsoleChat.exe pub blobtastic <AblyApiKey>
    ```

    > Ably will create a new channel if it doesn't yet exist.
