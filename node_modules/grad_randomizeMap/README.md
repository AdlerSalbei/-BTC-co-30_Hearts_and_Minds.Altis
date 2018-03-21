![alt text](https://imgur.com/V2xXenb.png)

## Description
This module changes the color of Buildings on the Following maps:
- Altis 
- Stratis

## Installation
### Manually
1. Create a folder in your mission root folder and name it `modules`. Then create one inside there and call it `grad-gpsTracker`.
2. Download the contents of this repository ( there's a download link at the side ) and put it into the directory you just created.
3. Append the following lines of code to the `description.ext`:

```sqf
class CfgFunctions {
    #include "modules\grad-gpsTracker\cfgFunctions.hpp"
};
```

## Configuration

### description.ext

Add the following:
```#include "node_modules\grad_randomizeMap\cfgLists.hpp"```

And to th cfgFunctions
```#include "node_modules\grad_randomizeMap\cfgFunctions.hpp"```

### initServer.sqf
Add the following:
```[Positon, Range] call grad_randomizeMap_fnc_colorBuildings;```
