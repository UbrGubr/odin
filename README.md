# odin - it's a thing

# Device Registry Service
## Usage

All responses will have the form
json
{
    "data": "Mixed type holding the content of the response",
    "message": "Description of what happened"
}

We will just describe what's going to appear in the `data field`

### List all devices

**Definition**

    `Get /devices`

**Response**

    `200 0K` on success

json
[
    {
        "identifier": "desktop",
        "name": "Desktop PC",
        "device_type": "computer",
        "controller_gateway": "192.1.168.0.2"
    },
    {
        "identifier": "main-tv",
        "name": "Living Room TV",
        "device_type": "tv",
        "controller_gateway": "192.168.0.9"
    }
]
