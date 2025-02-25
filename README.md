# Business Analyzer (Python)

## Overview

The **Business Analyzer** is a Python program designed to:

- Retrieve Business Data: Gather information about businesses based on a specified town, county, state, and business type using the Google Places and Google Geocoding API.
- Fetch Census Data: Obtain migration and demographic data from the US Census Bureau using the provided town, county, and state information.
- Visualize Data: Display all businesses within a given radius on a map.
- Generate Reports: Compile all results into a Microsoft Word document.
- The program performs statistical analysis on various business attributes, including opening hours, Google reviews/ratings, and offered services for specific business types within a town, county, and state in the United States.

**Note:** The US Census Bureau API may not return data for certain towns due to population constraints, which could lead to errors.

## API Keys

Links to sites to get API keys, none is needed for the US census but one is required for the Google API:

Google: https://developers.google.com/maps/documentation/javascript/get-api-key

US Census: https://api.census.gov/data/key_signup.html

Google API Documentation: https://developers.google.com/maps/documentation/places/web-service/details

US Census API Documentation: https://www.census.gov/data/developers/guidance/api-user-guide.html

Once you obtain your Google API key - put it in side the file marked "key.txt" so that it can be read into the program.

Usage:
```
python3 main.py -k key.txt -l "Albany, New York" -r 4000 -t cafe -c "Albany County" -s "New York"
```

Parameters:

-k key.txt: File containing your Google API key.

-l "Albany, New York": Location (town and state).

-r 4000: Radius in meters for business search.

-t cafe: Business type to search for.

-c "Albany County": County name.

-s "New York": State name.

## Example Output

Examples of results generated by the program can be found in the analysis_docs folder.
