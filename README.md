# Fundraising Pledge Management

Manage **`pledges`**, **`fundraisers`**, **`items`** and **`funds`** for fundraising campaigns 

**keyword `group`** 
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
        + ewaste: Type of electronic waste
        + status: Status of pledge : pending || adjusted || verified

## Update a pledge [POST]

## Create a new pledge [POST]

## Delete a pledge [POST]