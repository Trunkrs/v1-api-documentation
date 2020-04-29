# Best practices

There are several pointers which allow for a smooth integration:

## Cache the time slot endpoint

If you require the information of the time slot endpoint, to for instance create next day shipments, please cache this information. Time slots are only created at 2 AM so they are static during the day. A single request per day should be enough.

## Test your webhooks endpoint

If you opt to use webhooks: make sure you are returning a valid success response. If not this might lead to the disabling of your webhook.

## Use unique order references

Order references are used to track back parcels and, alternatively, as barcodes on non-Trunkrs labels. They need to be unique. If necessary pre-prend them with your company name.

## Cancel non-shipped shipments

Because of Trunkrs' unique fast delivery system, every booked shipment will be planned into tours (even if it doesnt arrive). Shipments which are not cancelled before 14:00 of the day of delivery and fail to arrive on the correct day, may be billed.