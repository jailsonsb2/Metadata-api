## Radio Metadata API

Get real-time metadata from online radio streams!

### How to Use:

1. **Start Monitoring:** Use the `/start_monitoring/` endpoint to begin tracking a radio station. 
   - **Example:** `https:twj.es/start_monitoring/?radio_url=https://example.com/stream` 

2. **Get Radio Information:** Once monitoring is started, access the `/radio_info/` endpoint for real-time metadata and history.
   - **Example:** `https:twj.es/radio_info/?radio_url=https://example.com/stream`
     
3. **Get Radio Complete Histoy:** Once monitoring is started, access the `/radio_histoy/` endpoint for complete history.
   - **Example:** `https://twj.es/radio_history/?radio_url=https://example.com/stream`

### Available Endpoints:

* `/start_monitoring/` **(GET):** Starts monitoring a radio stream. You must start monitoring before retrieving information.
    - **Required Parameter:** `radio_url`: The URL of the radio stream. 
* `/get_stream_title/` **(GET):** Retrieves the current song's title and album art from the radio stream.
    - **Required Parameter:** `url`: The URL of the radio stream. 
* `/radio_info/` **(GET):** Provides real-time information about the radio station, including the currently playing song and recent history.
    - **Required Parameter:** `radio_url`: The URL of the radio stream. 
* `/radio_history/` **(GET):** Fetches the complete song history from the database for a given radio station. You can set an optional limit on the number of records returned.
    - **Required Parameter:** `radio_url`: The URL of the radio stream.
    - **Optional Parameter:** `limit`: The maximum number of records to return.

### Contact

contato@jailson.es
