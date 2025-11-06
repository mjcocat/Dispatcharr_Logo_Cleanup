This plugin removes logos from the Dispatcharr database based on your preferences.

## Features
- Delete logos with NO relationships at all (completely unused)
- Delete VOD-only logos (logos not used by any channels)
- Preserves all channel logos
- Batch processing for large datasets (90k+ logos)
- Optional: Delete local logo files from disk
- Detailed logging and progress reporting

## Usage
1. Enable the plugin in the Plugins page
2. Choose your cleanup mode:
   - **Delete VOD-only logos**: ✅ ON = Delete logos only used by movies/series (keeps channel logos)
   - **Delete VOD-only logos**: ❌ OFF = Only delete logos with no relationships at all
3. Click "Run" to execute cleanup
4. Watch docker logs for progress: `docker logs -f dispatcharr`

## Settings
- **Delete VOD-only logos**: Remove logos only used by movies/series (default: false)
- **Delete local files**: Remove logo files from disk (default: false)
- **Batch size**: Number of logos to process at once (default: 5000)
