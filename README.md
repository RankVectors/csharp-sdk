# RankVectors C# SDK

[![NuGet Version](https://img.shields.io/nuget/v/RankVectors.svg)](https://www.nuget.org/packages/RankVectors)
[![NuGet Downloads](https://img.shields.io/nuget/dt/RankVectors.svg)](https://www.nuget.org/packages/RankVectors)

Official RankVectors API SDK for C# - Intelligent internal linking optimization using AI.

## Installation

Install via NuGet Package Manager:
```bash
Install-Package RankVectors
```

Or via .NET CLI:
```bash
dotnet add package RankVectors
```

Or via PackageReference:
```xml
<PackageReference Include="RankVectors" Version="1.0.0" />
```

## Quick Start

```csharp
using RankVectors.Client;
using RankVectors.com.rankvectors.api;
using RankVectors.com.rankvectors.model;

// Initialize the API client
var hostConfig = new HostConfiguration
{
    BaseUrl = "https://api.rankvectors.com"
};
var apiKey = new ApiKeyToken("YOUR_API_KEY", TokenPosition.Header);

var projectsApi = new ProjectsApi(hostConfig);
projectsApi.ApiKey = apiKey;

// Create a project
var request = new CreateProjectRequest
{
    Name = "My Website",
    WebsiteUrl = "https://example.com"
};

var project = await projectsApi.CreateProjectAsync(request);
Console.WriteLine($"Created project: {project.Name}");
```

## Features

- **AI-Powered Analysis**: Uses OpenAI embeddings to find optimal linking opportunities
- **Smart Crawling**: Automatically crawls and analyzes your website content
- **Automated Implementation**: Implement links via webhooks or manual instructions
- **Credit-Based System**: Pay-per-use model with transparent pricing
- **Multi-Platform Support**: Works with any CMS or platform via REST API

## Requirements

- .NET 9.0 or later
- Active RankVectors API key

## Getting Started

1. Sign up for a [RankVectors account](https://rankvectors.com)
2. Get your API key from Settings → API Keys
3. Install the NuGet package
4. Start optimizing your internal linking!

## Documentation

- [API Documentation](https://rankvectors.com/docs)
- [GitHub Repository](https://github.com/RankVectors/csharp-sdk)
- [RankVectors Website](https://rankvectors.com)

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Support

- Email: tj@rankvectors.com
- Documentation: https://rankvectors.com/docs
- Issues: https://github.com/RankVectors/csharp-sdk/issues