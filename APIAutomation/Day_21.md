## Problem statement
Build a REST API mock server that will allow to manage pricing individually on machines remotely with the following:

Endpoints:
- GET /pricing-models returns all of the pricing models available for the system also returns the default pricing model in prices.json
- POST /pricing-models creates a new pricing model in the system returns the ID of the new pricing model to the caller
- GET /pricing-models/:pm-id get an individual pricing model include the price configurations for the pricing model. If the pricing model isn't found by pm-id it responds with not found.
- PUT /pricing-models/:pm-id updates an existing pricing model meta-data does not affect the pricing configurations for the pricing model
- GET /pricing-models/:pm-id/prices returns the prices configured for a specific pricing model
- POST /pricing-models/:pm-id/prices adds a new price configuration for a pricing model
- DELETE /pricing-models/:pm-id/prices/:price-id removes a price configuration from a pricing model if the pricing model isn't found by pm-id it responds with not found. if the price configuration isn't found by price-id it responds with not found
- PUT /machines/:machine-id/prices/:pm-id sets the pricing model for an individual machine to the one from pm-id. If the machine already has a pricing model, it is replaced by this one. If the machine isn't found by machine-id it responds with not found. If the pricing model isn't found by pm-id it responds with not found
- DELETE /machines/:machine-id/prices/:pm-id removes the pricing model from the machine (unsets it)
- GET /machines/:machine-id/prices return the pricing model and price configurations set for a given machine.If the machine does not have a pricing model configured then the default model from prices.json is returned.If the machine isn't found by machine-id it responds with not found.
