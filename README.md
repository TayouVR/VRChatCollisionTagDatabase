# VRChat Collision Tag Database

This repo is designed to keep custom user made collision tags neatly organized and would allow anyone to contribute

The format in the various files is json based and structured like follows:


#### generic.json:
```json
{
    "name": "generic",
    "description": "General purpose tags, that might be useful for various random things",
    "entries": [
        {
            "tag": "Fire",
            "description": "This tag sets things on fire",
            "categories": {
                "generic"
            },
            "alternatives": {
                "fire",
                "flame"
            }
        }
        {
            "tag": "Electricity",
            "description": "Electricity",
            "categories": {
                "generic"
            },
            "alternatives": {
                "fire",
                "flame"
            }
        }
    ]
}
```

The following sample file stores all available json json files with tags conforming to the standard, that should be available when searching through them.
#### registry.json:
```json
{
    "registryName": "TayouVR (Use the repository or user name when defining this)",
    "libraries": [
        {
            "name": "Generic",
            "url": "https://github.com/TayouVR/VRChatCollisionTagDatabase/Path/To/File"
        },
        {
            "name": "Fighting",
            "url": "https://github.com/TayouVR/VRChatCollisionTagDatabase/Path/To/File"
        },
    ]
}
```

The editor extension will then take the path to such a registry file (can also be local) and use it to find any libraries, that conform tothe standard. 
These libraries can then be browsed through right in unity.


### These specs are Prototype specs and the editor script as of this point is not functional
https://github.com/TayouVR/VRChatCollisionTagExplorer
