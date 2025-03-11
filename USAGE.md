<!-- Start SDK Example Usage [usage] -->
```python
# Synchronous Example
from rapidapi_realtor_search_client import RapidapiRealtorSearchClient


with RapidapiRealtorSearchClient(
    api_key_auth="<YOUR_API_KEY>",
) as rrsc_client:

    res = rrsc_client.properties.search_buy(location="<value>")

    # Handle response
    print(res)
```

</br>

The same SDK client can also be used to make asychronous requests by importing asyncio.
```python
# Asynchronous Example
import asyncio
from rapidapi_realtor_search_client import RapidapiRealtorSearchClient

async def main():

    async with RapidapiRealtorSearchClient(
        api_key_auth="<YOUR_API_KEY>",
    ) as rrsc_client:

        res = await rrsc_client.properties.search_buy_async(location="<value>")

        # Handle response
        print(res)

asyncio.run(main())
```
<!-- End SDK Example Usage [usage] -->