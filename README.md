
# qb-gangs used with QBCore Framework
# Dependencies
* [qbcore framework](https://github.com/qbcore-framework)
* [qb-core](https://github.com/qbcore-framework/qb-core)
## Installation
### Manual
- Download the script and put it in the `[qb]` directory.
- Add the following code to your server.cfg/resouces.cfg
```
ensure qb-core
ensure qb-logs
ensure qb-gangs
ensure qb-radio
ensure qb-drugs
```

## Configuration
```
Config = Config or {}

Config.Fuel = 'ps-fuel' --ps-fuel, lj-fuel, LegacyFuel

Config.stash ={
    ["ballas"] = vector3(113.3059, -1970.89, 21.3276),
    ["vagos"] = vector3(344.67, -2022.14, 22.39),
    ["families"] = vector3(-136.91, -1609.84, 35.03),
}

Config.Gangs = {
    ["ballas"] = {
        ["VehicleSpawner"] = vector4(108.58, -1945.01, 20.8, 43.42),
        ["colors"] = { 145, 0 }, ---  primary and secondary colors id https://wiki.rage.mp/index.php?title=Vehicle_Colors
        ["vehicles"] = {
            ["buffalo2"] = "Buffalo Sport",
            ["rumpo3"] = "RumpoXL",
            ["manchez"] = "Manchez",
            ["chino2"] = "Lowrider",
        },
    },
    ["vagos"] = {
        ["VehicleSpawner"] = vector4(329.59, -2035.1, 20.98, 53.08),
        ["colors"] = { 89, 0 }, ---  primary and secondary colors id https://wiki.rage.mp/index.php?title=Vehicle_Colors
        ["vehicles"] = {
            ["buffalo2"] = "Buffalo Sport",
            ["rumpo3"] = "RumpoXL",
            ["manchez"] = "Manchez",
            ["chino2"] = "Lowrider",
        },
    },
    ["families"] = {
        ["VehicleSpawner"] = vector4(-108.68, -1598.61, 31.66, 329.64),
        ["colors"] = { 53, 0 }, ---  primary and secondary colors id https://wiki.rage.mp/index.php?title=Vehicle_Colors
        ["vehicles"] = {
            ["buffalo2"] = "Buffalo Sport",
            ["rumpo3"] = "RumpoXL",
            ["manchez"] = "Manchez",
            ["chino2"] = "Lowrider",
        },
    },  -- Add your next table under this comma
}
