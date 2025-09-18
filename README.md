# Query-Google-Places-API
_Querying Google Places API_

```bash

$ curl -X POST -d '{
                             "textQuery" : "sapatos goiania, goias."
                           }' \
                               -H 'Content-Type: application/json' -H 'X-Goog-Api-Key: your-api-key-here' \
                               -H 'X-Goog-FieldMask: places.displayName,places.formattedAddress,places.location,places.priceLevel' \
                               'https://places.googleapis.com/v1/places:searchText'

{
  "places": [
    {
      "formattedAddress": "R. 1130, 145 - St. Marista, Goiânia - GO, 74180-090, Brazil",
      "location": {
        "latitude": -16.7017704,
        "longitude": -49.2613919
      },
      "displayName": {
        "text": "Empório Shoes",
        "languageCode": "pt"
      }
    },
    {
      "formattedAddress": "R. T-47, 19 - St. Oeste, Goiânia - GO, 74140-120, Brazil",
      "location": {
        "latitude": -16.6872999,
        "longitude": -49.2744912
      },
      "displayName": {
        "text": "Closet 35 - Loja de Calçados e bolsas em Goiânia - Só vendemos numeração 35",
        "languageCode": "en"
      }
    },
    {
      "formattedAddress": "R. C-136, 718 - Jardim América, Goiânia - GO, 74275-050, Brazil",
      "location": {
        "latitude": -16.7118541,
        "longitude": -49.2832833
      },
      "displayName": {
        "text": "Ana Paula Calçados",
        "languageCode": "pt"
      }
    },

    ...




```

## Outros valores para o X-Goog-FieldMask 

_rating_: The overall user rating of the place. <br>
_user_ratings_total_: The total number of reviews for the place. <br>
_photos_: An array of photo objects, each with a reference to an image.    <br>
.... <br> 

*Juices....* 
