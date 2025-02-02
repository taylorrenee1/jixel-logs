﻿
# Jixel-Logs

[![Version](https://img.shields.io/badge/version-1.0.0-brightgreen.svg)](https://github.com/yourusername/repo/releases)

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Previews](#previews)
- [Support](#support)
- [License](#license)

## Description

This is to replace logs from QB-SmallResources, so you can hot ensure your logs.

You should still use a logging service as Discord is not a logging service and will rate limit you.


## Installation

1. Download the latest release from the [Releases](https://github.com/taylorrenee1/jixel-logs/releases) page.
2. Extract the files into your `resources` folder. or `standalone`
3. Add the resource to your `server.cfg`:

    ```lua
    ensure jixel-logs
    ```

## Configuration

It pretty much is plug and play - except for the need to change a few things.

1) Change SERVERNAME in the `logs.lua` to your server Name

2) Change icon_url to imgur or imgbb link of your server logo

3) Add your webhook links to the `logs.lua`

### Usage
```lua
TriggerEvent('jixel-logs:server:CreateLog', 'logname', 'TitleofLog', 'color', 'Message', 'tageveryone true or false')
```
Example usage:

```lua
TriggerEvent('jixel-logs:server:CreateLog', 'me', 'ME', 'white', '**' .. GetPlayerName(source) .. '** (CitizenID: ' .. Player.PlayerData.citizenid .. ' | ID: ' .. source .. ') **Message:** ' .. text, false)
```


## Previews

### Example
![Example of Discord Log](https://i.ibb.co/983Jd82/image.png)


## Support

For support, join the [Discord](https://discord.gg/jixelpatterns)

For other scripts visit our [Tebex Store](https://jixeltay.tebex.io).

