# Frank-Energie
API call for Frank Energie dynamic market prices (Electricity & Gas)

Use GraphQL

query MarketPrices {
    marketPrices(date: "2024-06-08") {
        electricityPrices {
            from
            till
            marketPrice
            marketPriceTax
            sourcingMarkupPrice
            energyTaxPrice
            perUnit
        }
        gasPrices {
            from
            till
            marketPrice
            marketPriceTax
            sourcingMarkupPrice
            energyTaxPrice
            perUnit
        }
    }
}

Endpoint: https://graphql.frankenergie.nl/ <br>
To filter for a country for example BE, add a header<br>
x-country with value BE<br><br>
More info: https://reversed.notion.site/Marktprijzen-API-89ce600a88ac4abe8c2ad89d3167a83e
