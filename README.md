# AbyssalSpotify
A Spotify API wrapper for .NET Standard 2.1 (written in C#).
  
## Build Status
| Pipeline status | Latest stable | Latest pre-release |
|---------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------------------------------------|
| [![Build Status](https://dev.azure.com/abyssal512/AbyssalSpotify/_apis/build/status/abyssal512.AbyssalSpotify?branchName=master)](https://dev.azure.com/abyssal512/AbyssalSpotify/_build?definitionId=1) | [![Nuget](https://img.shields.io/nuget/v/AbyssalSpotify.svg)](https://www.nuget.org/packages/AbyssalSpotify/) | [![Nuget (with prereleases)](https://img.shields.io/nuget/vpre/AbyssalSpotify.svg)](https://www.nuget.org/packages/AbyssalSpotify/) |  

Currently, there are no stable releases, although the latest pre-release is fairly stable and should work in your production builds. When updating, always check the commit notes. 
  
## Motivation
When I used SpotifyAPI-NET, I found that a lot of the code didn't seem very professional and didn't follow C# design principles and philsophy, and I was very annoyed at the fact that the client didn't automatically reauthorize for client credential authorizers, meaning that I had to re-authorize manually when the key expired. AbyssalSpotify is designed to be extremely powerful, yet extremely simple to use, so that all authorization code is handled automatically for you. I also endeavour to provide high-quality, correct English-language documentation with *every* method, parameter, class, and public-facing object in the library, to provide top-tier user friendliness. 
That being said, AbyssalSpotify is still very early in development, and lacks a significant portion of the advanced features SpotifyAPI-NET has.

## Usage
Documentation is a work-in-progress. You can see `AbyssalSpotify.Tests\Program.cs` for a brief example, 
but XML documentation is included with all public-facing classes and methods. You can also generate the documentation using DocFX and browse it locally. If you have any issues, feel free to open a GitHub issue.

## Feature Roadmap
* [x] Authentication
  * [x] Client Credentials authentication flow
  * [ ] Implicit Grant
  * [ ] Authorization Code
* [x] Tracks
  * [x] Track references
  * [x] Dereferencing
* [x] Albums
  * [x] Album references
  * [x] Dereferencing
* [x] Querying
  * [x] Mixed querying
  * [x] Selective querying
  * [x] Pagination querying
    * [ ] Use `IAsyncEnumerable<T>`

* [ ] Ratelimits (429 Too Many Requests and `Retry-After`)
* [ ] Playlists
* [ ] Player
* [ ] Personalization
* [ ] Categories
* [ ] Users
* [ ] Conditional requests (Cache-Control)


## Examples
AbyssalSpotify is used extensively in some of my other projects, namely [Abyss](https://github.com/abyssal/Abyss), a Discord bot.
  
## Copyright  
Copyright (c) 2019 Abyssal.  
Spotify application and API is Copyright (c) 2019 Spotify Technology S.A.   
All media and content belongs to their respective owners.  
