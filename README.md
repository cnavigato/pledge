# Fundraising Pledge Management

Manage **`pledges`**, **`fundraisers`**, **`items`** and **`funds`** for fundraising campaigns 

# Pledges [/pledges/{id}]

+ Parameters

    + id: abc123 (required) - Unique identifier for a pledge

## Get a pledge [GET]
Gets a single pledge by its unique identifier.

+ Response 200 (application/json)

    + Attributes

        + id: abc123
        + fundrasierid: This is a fundraiser identifier
        + timestamp: Time of the pledge
        + name: Name of pledger
        + email: Email of pledger
        + phone: Phone number of pledger
        + address: Address of pledger
        + itemType: Type of item pledged
        + status: Status of pledge : pending || adjusted || verified

## Update a pledge [POST]
Modify a `pledges'` data using its unique identifier. You can edit the `name`, `email`,`address`,`itemType`, and `status`.

+ Request (application/json)

    + Attributes

        + name: Name of pledger
        + email: Email of pledger
        + phone: Phone number of pledger
        + address: Address of pledger
        + itemType: Type of item pledged
        + status: Status of pledge : pending || adjusted || verified

    + Schema

            {
                "type": "object",
                "description": "Update a pledge",
                "properties": {
                    "name": {
                        "type": "string"
                    },
                    "email": {
                        "type": "string"
                    },
                    "phone": {
                        "type": "string"
                    },
                    "address": {
                        "type": "string"
                    },
                    "itemType": {
                        "type": "string"
                    },
                    "status": {
                        "type": "array",
                        "items": {
                            "type": "string"
                        }
                    }
                },
                "additionalProperties": false
            }

+ Response 204

## Create a new pledge [POST]

## Delete a pledge [POST]