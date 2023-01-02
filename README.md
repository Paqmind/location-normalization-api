# API for normalizing location data from String to Object

Use cases:
* organize user location data in a searchable format
* normalize the analyzed data
* Google Maps alternative to get full location based on inputted data


## How it works

|  Input                            |  API Response                                                                               | 
|-----------------------------------|---------------------------------------------------------------------------------------------|
| San Francisco                     | `{"country": "United States of America", "region": "California", "city": "San Francisco"}` | 
| San Francisco, USA                | `{"country": "United States of America", "region": "California", "city": "San Francisco"}` | 
| San Francisco - USA               | `{"country": "United States of America", "region": "California", "city":" San Francisco"}` | 
| San Francisco [USA]               | `{"country": "United States of America", "region": "California", "city": "San Francisco"}` | 
| San Francisco ❤️                   | `{"country":" United States of America", "region": "California", "city": "San Francisco"}` | 
| CA                                | `{"country": "United States of America", "region": "California"}`                          | 
| NY                                | `{"country": "United States of America", "region": "New York"}`                            | 
| NYC                               | `{"country": "United States of America", "region": "New York", "city": "New York City"}`   | 
| Rio de Janeiro                    | `{"country": "Brazil", "region": "Rio de Janeiro"}`                                        |  
| @São Paulo, Brazil                | `{"country": "Brazil", "region": "São Paulo"} `                                            | 

## Contact Us

Interested to get an access to the Location Normalization API? Contact us at info@paqmind.com
