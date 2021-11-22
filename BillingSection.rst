Billing section
===============



Billing Section gives the overall billing status of the products registered by the user in the portal.

We need to configure and set up an environment(both UI and API) for the billing section.

Environment setup(UI)
~~~~~~~~~~~~~~~~~~~~~

In order to set up the environment for the Duplication or Product Registration, after the successful setup process for the Compliance, we have to add additional credentials information in the different related domains.

#. Compliance-UI
    Add the private key for the Stripe in environment.ts
    stripe_pk: [Add the private key]

#. Compliance-api
   Set the following configurations to env.dev file
    ANNUAL_PRICING_KEY: [Add the annual_pricing_key]
    ANNUAL_WHITE_LABEL_PRODUCT_KEY:[Add the annual_white_label_product_key]
    AUTH0_ORIGIN: https://login.staging.sorting.tech/
    AUTH0_JWT_AUDIENCE: https://compliance-api.staging.sorting.tech/
    AUTH0_INTERNAL_CONNECTION_NAME: portal-staging-db
    INTERNAL_BINNING_DOMAIN: http://api-binning.binning.svc.cluster.local:5000/
    STRIPE_API_KEY: [Add the stripe_api_key]
    TAXJAR_API_KEY: [Add the taxjar_api_key]
    LEGACY_ANNUAL_PRICING_KEY:[Add pricing key values for legacy annual subscription] 
    PROMOTIONAL_ANNUAL_PRICING_KEY:[Add pricing key for promotional subscription]
#. Rails -admin
    On the Supplier associated with the current user set the following credentials:

    * state: AK
    * country:US
    * Zip: 99501
On the /billing-info section, set the credit card number into 42424242424242, the value of the billing_customer and billing_type gets set on the suppliers section, which helps to bypass the payment section while performing the tests.
