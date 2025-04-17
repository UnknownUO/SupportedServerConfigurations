# Supported Server Configurations

This repository is used to host the JSON list of supported shards for MobileUO

## How to add your shard

To get your shard added to the list of supported shards for MobileUO, create a new PR to this repo by modifying the `SupportedServerConfigurations.json` with the following information:

```
{
    "Name":"Renaissance",
    "UoServerUrl":"login.uorenaissance.com",
    "UoServerPort":"2593",
    "FileDownloadServerUrl":"uorenaissance.com",
    "FileDownloadServerPort":"80",
    "ClientVersion":"5.0.8.3",
    "UseEncryption":false,
    "ClientPathForUnityEditor":"",
    "AllFilesDownloaded":false,
    "PreferExternalStorage":false,
    "SupportedServer":true
  },
```

Please keep the list sorted alphabetically by Name.

**Name:** The name of your shard

**UoServerUrl:** the URL to connect to your shard

**UoServerPort:** the port to connect to your shard

**FileDownloadServerUrl:** the URL of where to download the game data files. You can either standup a webserver that hosts the individual gamedata files OR you can create a single .zip file that contains everything in it. **We recommend using a zip file.** You must host the game data files for your shard, do not use another shard's game data fles

**FileDownloadServerPort:** the port of where to download the game data files

**ClientVersion:** the UO version of your game data files

**UseEncryption:** leave false

**ClientPathForUnityEditor:** used for development, leave blank

**AllFilesDownloaded:** leave false

**PreferExternalStorage:** leave false

**SupportedServer:** leave true

We will review your shard's configuration before approving and merging your PR. Once merged, all MobileUO user's will see the shard listed under supported shards.
