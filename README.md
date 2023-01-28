# CurrentWeather_ByCity
A UiPath Automation that utilizes the OpenWeather API to fetch the current weather conditions of US cities listed in an Excel sheet, then populates the data into the Excel sheet. 

To use this automation, create an account with https://openweathermap.org to gain access to the free API key. You'll need to plug this API key into the "ApiKey" variable within
the HTTP Request activity. You'll then need to find the Excel datasheet within the ".data" project folder. This folder contains some preset data -- feel free to replace with
your own. 

The automation will scrape the city names from the datasheet and request current weather conditions from the OpenWeather API, and then write those conditions back into the Excel
data sheet in their respective columns. If for some reason weather conditions cannot be found for a specified city, the automation will handle the error and input "Not Found"
into the spreadsheet. Happy automating! 
