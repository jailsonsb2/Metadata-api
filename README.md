## Radio Metadata API

Get real-time metadata from online radio streams!

### How to Use

**API Overview:**
Our API provides detailed radio information, including current song details, song history, album art, and more. The API has two main endpoints:

1. **`/get_stream_title/`**
   - **Parameter:** `url` (the URL of the radio stream)
   - **Example:** `https://twj.es/get_stream_title/?url=https://stream.zeno.fm/yn65fsaurfhvv`

2. **`/radio_info/`**
   - **Parameter:** `radio_url` (the URL of the radio stream)
   - **Example:** `https://twj.es/radio_info/?radio_url=https://stream.zeno.fm/yn65fsaurfhvv`

### Example Player

For a practical implementation, you can refer to a free radio player that is already updated to work with this API. Check it out here: [RadioPlayer on GitHub](https://github.com/jailsonsb2/RadioPlayer). This example player includes built-in functionality to handle API requests and keep the metadata current.

### Contact

For any questions or further assistance, please contact us at: [contato@jailson.es](mailto:contato@jailson.es)

Feel free to reach out if you need help with implementing or using the API!
