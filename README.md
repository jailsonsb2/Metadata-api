## Radio Metadata API

Get real-time metadata from online radio streams!

### How to Use

**API Overview:**
Our API provides detailed radio information, including current song details, song history, album art, and more. The API has two main endpoints:

1. **`/get_stream_title/`**
   - **Purpose:** Updates the song history and the last played song in the database.
   - **Parameter:** `url` (the URL of the radio stream)
   - **Example:** `https://twj.es/get_stream_title/?url=https://stream.zeno.fm/yn65fsaurfhvv`

2. **`/radio_info/`**
   - **Purpose:** Retrieves the last played song and the song history for a given radio stream.
   - **Parameter:** `radio_url` (the URL of the radio stream)
   - **Example:** `https://twj.es/radio_info/?radio_url=https://stream.zeno.fm/yn65fsaurfhvv`

### How It Works

1. **Updating Metadata:**
   - The `/get_stream_title/` endpoint is designed to update the database with the current song's information. This endpoint should be called periodically to keep the song history current. Typically, this is handled by a client-side script running on the player that makes these requests.

2. **Retrieving Information:**
   - The `/radio_info/` endpoint allows you to query the database for the last played song and the song history. This endpoint provides a JSON response containing this data.

### Important Note

The `/get_stream_title/` endpoint, which updates the metadata, is intended to be called regularly by a client-side script. This script should run on the player's environment, ensuring that the database is continuously updated with the latest song information. As users listen to the radio, the script makes requests to keep the song history up-to-date.

### Contact

For any questions or further assistance, please contact us at: [contato@jailson.es](mailto:contato@jailson.es)

Feel free to reach out if you need help with implementing or using the API!
