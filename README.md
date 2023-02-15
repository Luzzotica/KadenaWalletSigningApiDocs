# An Open API Spec for the Kadena Wallet Signing Api

The `swagger.yaml` file contains the OpenAPI spec for the Kadena Wallet Signing Api.
This can be used by redocly (Kadena's current OpenAPI spec generator) to build a beautiful webpage for it.

# Some Notes

I decided to combine the QuicksignSigner and the normal Signer into one model as Alber mentioned in the KIP.  
This is so that the Signer object can be used in both Quicksign and Sign endpoints.  
All that this required was making both the `public` and `sig` fields nullable. 

Currently, all of the models are there, and the `\sign` and `\quicksign` endpoints are defined using those models.  

# Contributing

The things that still need doing:

- Examples, specifically of things like continuation commands
- Improved descriptions