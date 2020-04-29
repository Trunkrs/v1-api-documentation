# Intro

The Trunkrs API is designed for Trunkrs clients to create shipments and retrieve statusses. If you are not yet a Trunkrs customer and would like to become one, please visit our website https://www.trunkrs.nl

## Authentication

Authentication is done via two headers:

- x-api-clientid
- x-api-clientsecret

*Please note: the credentials between staging and production differ, please use the correct credentials*

## Content type when posting

whenever we require a payload (such as in creating a shipment) we expect this as content-type: application/json

## Questions?

Please contact tech.support@trunkrs.nl