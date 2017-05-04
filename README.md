{
  "swagger": "2.0",
  "info": {
    "version": "1.0",
    "title": "WeatherAPI",
    "x-lastModified": "Jan 25, 2017 09:34AM PST"
  },
  "paths": {
    "/CityWeatherByZip/{ZipCode}": {
      "get": {
        "produces": [
          "application/json",
          "application/xml"
        ],
        "responses": {
          "200": {
            "description": "Success response",
            "schema": {
              "$ref": "#/definitions/WeatherResponseSchema"
            }
          }
        },
        "parameters": [
          {
            "name": "ZipCode",
            "in": "path",
            "description": "",
            "required": true,
            "type": "string",
            "format": ""
          }
        ]
      }
    }
  },
  "definitions": {
    "WeatherResponseSchema": {
      "title": "WeatherSchema",
      "type": "object",
      "properties": {
        "city": {
          "type": "string"
        },
        "temperature": {
          "type": "string"
        },
        "wind": {
          "type": "string"
        },
        "clouds": {
          "type": "string"
        },
        "forecast": {
          "type": "string"
        }
      }
    }
  }
}