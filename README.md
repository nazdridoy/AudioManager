# AudioManager
AudioManager is a versatile command-line tool for managing audio files. It supports converting audio formats, transferring metadata, and cleaning up audio files. The tool is designed to work with `.weba`, `.opus`, and `.m4a` file types.

## Features

- **Convert WEBA to OPUS**: Easily convert `.weba` files to `.opus` format.
- **Transfer Metadata**: Transfer metadata and cover art from `.m4a` files to `.opus` files.
- **File Cleanup**: Remove unwanted audio files by type.
- **Detailed File Information**: Display detailed information about audio files.
- **Single File and Directory Processing**: Process individual files or entire directories.

## Dependencies

AudioManager requires the following dependencies:

- `ffmpeg`: For audio conversion and metadata handling.
- `kid3-cli`: For managing cover art.
- `jq`: For processing JSON data.

Ensure these dependencies are installed on your system before using AudioManager.

## Installation

Clone the repository to your local machine:
```bash
git clone https://github.com/nazdridoy/AudioManager.git
cd AudioManager
```
Make the script executable:
```bash
chmod +x AudioManager
```

## Usage

Run the script with the desired options and path:
```bash
./AudioManager [OPTIONS] [PATH]
```

### Options

- `-h, --help`: Show help information.

### Arguments

- `PATH`: Path to a directory or single audio file. If not provided, the current directory is used.

### Examples

- Process the current directory:

  ```bash
  ./AudioManager
  ```

- Process a specific directory:

  ```bash
  ./AudioManager /path/to/music
  ```

- Process a single file:

  ```bash
  ./AudioManager /path/to/song.opus
  ```

- Show help:

  ```bash
  ./AudioManager -h
  ```

## Notes

- When processing a single file, the script will look for matching files with the same name but different extensions.
- Backup important files before performing operations.
- Use the cleanup option with caution.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

THIS IS A PERSONAL PROJECT BUT Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## Contact

For questions or suggestions, please open an issue on GitHub.
